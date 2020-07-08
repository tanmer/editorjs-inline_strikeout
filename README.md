# Strikeout Tool
Inline tool for strikeout text fragments for the [Editor.js](https://github.com/codex-team/editor.js)


### Download to your project's source dir

1. Upload folder `dist` from repository
2. Add `dist/bundle.js` file to your page.

## Usage

Add a new Tool to the `tools` property of the Editor.js initial config.

```javascript
import EditorJs from '@editorjs/editorjs';
import InlineStrikeout from 'editorjs-inline_strikeout';

var editor = new EditorJS({
  // ...
  tools: {
    // ...
    strikeout: InlineStrikeout
  },
});
```

## Config Params

This Tool has no config params

## Output data

Underlined text will be wrapped with a `strikeout` tag with an `cdx-del` class.

```json
{
    "type" : "text",
    "data" : {
        "text" : "Create a directory for your module, enter it and run <del class=\"cdx-del\">npm init</del> command."
    }
}
```
