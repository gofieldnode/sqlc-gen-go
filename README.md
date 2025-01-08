# sqlc-gen-go

This is a modified version of the original `sqlc-gen-go` plugin. It is used by some Fieldnode
projects and is not meant to be used outside the organization.

## Modification

The following modification has been done:

* All methods and types are prefixed with `db`. This is to make ensure its not exported outside package.
* `DBTX` is renamed to `dbExecutor`.
* Copy is not generated event if turned on.
* Batch code generation is not generated even if turned on.
* Interfaces are not generated even if turned on.
* Query code is not recognizing `EmitMethodsWithDBArgument` setting.
