# Operator-caska Cursive Font
Font with ligature and cursive support, combination of both **CaskaydiaCove Nerd Font** and **Operator Mono**.

![image](https://github.com/Anant-mishra1729/Operator-caska-Font/assets/84588156/bb718779-5a6f-44e5-8c05-313c67b583e8)

<p align = "center"><b>Operator-caskabold</b> with <a href = "https://vscodethemes.com/e/iamkd.one-monokai-italics/one-monokai-italics">One Monokai Theme with Italics - Danyil Karuna</a> </p>

## Usage
Use a theme that supports italics, such as **Monokai Pro**.
### 📖 Book italics (Default)
Font family: **`Operator-caska`**.
### 💪 Bold italics
Font family: **`Operator-caskabold`**.

## Installation
Clone this repo:
```sh
git clone https://github.com/Anant-mishra1729/Operator-caska-Font.git
cd Operator-caska-Font
```

### Linux
* Create a directory named **`.fonts`** in your HOME directory:
```sh
mkdir -p ~/.fonts
```
* Copy the .ttf files in your ~/.fonts directory
```sh
cp -r *.ttf ~/.fonts/
```

### Windows
Install the fonts by right-clicking the .ttf files.

<hr>

### Issues
* **Operator-caskabold in Windows**: VScode font is not cursive (Issue only with Windows)

You'll have to **[modify the textmate rules](https://code.visualstudio.com/api/language-extensions/syntax-highlight-guide)**, here's an example, paste this in **settings.json**

```js
"editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "scope": [
          "comment",
          "entity.name.type.class", // class names
          "keyword", // import, export, return
          "constant", // String, Number, Boolean..., this, super
          "storage.type",
          "variable.language.this.cpp"
        ],
        "settings": {
          "fontStyle": "italic bold" // comments are italic
        }
      },
    ]
  },
```

**Output**
|Without textmate rules|With textmate rules|
|-|-|
|![image](https://github.com/Anant-mishra1729/Operator-caska-Font/assets/84588156/ab06dbfd-9218-4544-9690-eb3e48ee4633)|![image](https://github.com/Anant-mishra1729/Operator-caska-Font/assets/84588156/e7d69e5a-a31f-4b27-b967-39dc1ba3a44d)|


