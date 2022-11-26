<h1 align="Center">
    Change specific items of a Theme in VSCode
</h1>

<img align="right" src="../VSCode-Color-Theme/images/settings-json.png">

- First, open ``Settings`` in VSCode (Hotkey: ``CTRL / CMD + ,``)
- Click on the button in the right upper corner to open up ``settings.json``
- Then add your changes in the color (examples further down below)

The changes will effect **all** color Themes!

<h2 align="center">
    Examples:
</h2>

If not already, you need to add ``"editor.tokenColorCustomizations": {}`` anywhere in the file.
There are variations of commands, to change the syntax colors!

<br>

<p align="center">To change the color of strings:</p>

```json
"editor.tokenColorCustomizations": {
    "strings": "#12a95c",
},
```
<br>

<p align="center">To change the color of comments:</p>

```json
"editor.tokenColorCustomizations": {
    "comments": "#12a95c",
},
```
<br><br>

<h2 align="center">For the following codes, we will always be in the "textMateRules":</h2>

```json
"editor.tokenColorCustomizations": {
    "textMateRules": [
        {
            "scope": "entity.tag.name", // change this to whatever needed.
            "settings": {
                "foreground": "#12a95c" // change the color to whatever needed.
            }
        },
    ]
},
```
<br>

<p align="center">To change the color of quotation marks:</p>

```json
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
```

<br>

<p align="center">To change the color of classes in css (.body, etc.)</p>

```json
{
    "scope": "entity.other.attribute-name.class.css",
    "settings": {
        "foreground": "#05a1f7"
    }
},
```

<br>

<p align="center">To change the color of id's in css (#body, etc.)</p>

```json
{
    "scope": "entity.other.attribute-name.id.css",
    "settings": {
        "foreground": "#05a1f7"
    }
},
```
<br>

<p align="center">To change the color of classes in html</p>

```json
{
    "scope": "entity.other.attribute-name",
    "settings": {
        "foreground": "#05a1f7"
    }
},
```

<br>

<p align="center">To change the color of pseudo-elements in css (input::placeholder, etc.)</p>

```json
{
    "scope": "entity.other.attribute-name.pseudo-element",
    "settings": {
        "foreground": "#49AEE6"
    }
},
```

<br>

<p align="center">To change the color of pseudo-classes in css (button:hover, etc.)</p>

```json
{
    "scope": "entity.other.attribute-name.pseudo-class",
    "settings": {
        "foreground": "#49AEE6"
    }
},
```

<br>

<p align="center">To change the color of numbers (in css, for example)</p>

```json
{
    "scope": "constant.numeric",
    "settings": {
        "foreground": "#47d4b9"
    }
},
```

<br>

<p align="center">To change the color of units in css (px, rem, etc.)</p>

```json
{
    "scope": "keyword.other.unit",
    "settings": {
        "foreground": "#47d4b9"
    }
},
```

<br>

<p align="center">To change the color of (constant) rgb/hex-values (#fffff, etc.)</p>

    
```json
{
    "scope": "constant",
    "settings": {
        "foreground": "#47d4b9"
    }
},
```

<br>

<p align="center">To change the color of # in css (before the hex color-code), etc.</p>


```json
{
    "scope": "punctuation.definition.constant",
    "settings": {
        "foreground": "#47d4b9"
    }
},
```
