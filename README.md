# Sass Compilation Setup

Follow these steps to set up Sass compilation to a `dist/` folder.

### 1. Create the `dist/` Folder
In your project directory, create a `dist/` folder to store compiled CSS:

```bash
mkdir dist
```

### 2. Install Live Sass Compiler Extension in VSCode
Ensure the [Live Sass Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass) extension is installed.

### 3. Configure Output Path
To automatically save compiled CSS to `dist/`, create or edit `.vscode/settings.json` in your project root:

```json
{
  "liveSassCompile.settings.formats": [
    {
      "format": "expanded",
      "extensionName": ".css",
      "savePath": "/dist"
    }
  ]
}
```

### 4. Compile Sass
In VSCode, click **Watch Sass** in the bottom bar to compile your Sass files automatically to `dist/`.

