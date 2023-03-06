only main branch

```bash
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
```

```yml
settings:
    Actions:
        Workflow permissions: RW
    Pages:
        Build and deployment:
            Source: Deploy from a branch
            Branch: None
```
