#!groovy


properties([
    parameters([
        booleanParam(defaultValue: true,
                     description: 'Cancel the rest of parallel stages if one of them fails and return status immediately',
                     name: 'failFast'),
        booleanParam(defaultValue: true,
                     description: 'Propagate status to GitHub',
                     name: 'propagateStatus'),
        string(defaultValue: 'pull/826/head',
               description: 'Pipeline shared library version (branch/tag/commit). Determined automatically if empty',
               name: 'library_version')
    ])
])

loadOpenVinoLibrary {
    entrypoint(this)
}
