<h1 align="Center">
    Change specific items of a Theme in VSCode
</h1>

- First, open ``Settings`` in VSCode (Hotkey: ``CTRL / CMD + ,``)
- Click on the button in the right upper corner to open up ``settings.json``
- Then add your changes in the color (examples further down below)

The changes will effect **all** color Themes!

<h2 align="center">
    Examples:
</h2>

If not already, you need to add ``"editor.tokenColorCustomizations": {}`` anywhere to it.

To change the color of strings:
```json
"editor.tokenColorCustomizations": {
    "strings": "#12a95c",
},
```

To change the color of quotation marks:
```json
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": "punctuation.definition.string.begin",
            "settings": {
                "foreground": "#12a95c"
            }
        },
        {
            "scope": "punctuation.definition.string.end",
            "settings": {
                "foreground": "#12a95c"
            }
        },
    ]
},
```

To change the color of comments:
```json
"editor.tokenColorCustomizations": {
    "comments": "#12a95c",
},
```
