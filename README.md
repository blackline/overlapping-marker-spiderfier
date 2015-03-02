Update the Git tag
==================

    git checkout [your-branch-name]

    # List all of the git tags
    git tag

        1.0.1
        1.0.2
        1.0.3
        1.0.4
        1.0.5

    # Increment the patch version of the highest tag version
    git tag 1.0.6

    # Push up the new tag
    git push --tags origin

    # Finally, update your bower.json to point to the new tag version

    cat bower.json
        ...
        "overlappingmarkerspiderfier": "https://github.com/blackline/OverlappingMarkerSpiderfier.git#1.0.6",
        ...

    # Don't forget to update the dependencies
    sudo ant install-deps
