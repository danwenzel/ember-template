# ember-template

An ember starter app, that started with `ember new` and added some of my favorite ember things:

- prettier, embedded into eslint
- prettier for handlebars, with autofix

## auto-fixing templates in VS Code

- Install https://marketplace.visualstudio.com/items?itemName=emeraldwalk.RunOnSave
- Add the following to your VS Code `settings.json`:

```json
"emeraldwalk.runonsave": {
  "commands": [
    {
      "match": "\\.hbs$",
      "cmd": "yarn prettier ${file} --write --parser=glimmer"
    },
  ]
}
```
