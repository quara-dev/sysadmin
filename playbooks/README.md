# Collections Playbooks Directory

This directory can be used to ship various playbooks inside an Ansible collection.

In prior releases, you could reference playbooks in this directory using the full path to the playbook file from the command line.

Starting from `ansible-core>=2.11`, you can use the FQCN, `namespace.collection.playbook` (with or without extension), to reference the playbooks from the command line or from `import_playbook`.

> This will keep the playbook in ‘collection context’, as if you had added `collections: [ namespace.collection ]` to it.

You can have most of the subdirectories you would expect, such files/, vars/ or templates/ but no roles/ since those are handled already in the collection:

```
├── playbooks/
│   ├── files/
│   ├── vars/
│   ├── templates/
│   ├── tasks/
│   ├── some-playbook.yml
│   └── other-playbook.yml
```
