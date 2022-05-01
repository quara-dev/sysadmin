# Collections Role Directory

Collection roles are mostly the same as existing roles, but with a couple of limitations:

- Role names are now limited to contain only lowercase alphanumeric characters, plus `_` and start with an alpha character.

- Roles in a collection cannot contain plugins any more. Plugins must live in the collection plugins directory tree. Each plugin is accessible to all roles in the collection.

- The directory name of the role is used as the role name. Therefore, the directory name must comply with the above role name rules. The collection import into Galaxy will fail if a role name does not comply with these rules.

- You can migrate ‘traditional roles’ into a collection but they must follow the rules above. You may need to rename roles if they don’t conform. You will have to move or link any role-based plugins to the collection specific directories.
