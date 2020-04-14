# ember-template-1

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
