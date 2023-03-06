```bash
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
```

```yml
rule:
    branch: main
settings:
    Actions:
        Workflow permissions: default
    Pages:
        Build and deployment:
            Source: Deploy from a branch
            Branch: None
Actions:
    push:
        result: perm error
    pages build and deployment:
        result: success
        pages: README.md
```

```yml
rule:
    branch: main
settings:
    Actions:
        Workflow permissions: RW
    Pages:
        Build and deployment:
            Source: Deploy from a branch
            Branch: None
Actions:
    push:
        result: success
    pages build and deployment:
        result: success
        pages: README.md
```

```yml
rule:
    branch: main
    nojekyll: yes
settings:
    Actions:
        Workflow permissions: RW
    Pages:
        Build and deployment:
            Source: Deploy from a branch
            Branch: None
Actions:
    push:
        result: success
    pages build and deployment:
        result: success
        pages: 404
```
