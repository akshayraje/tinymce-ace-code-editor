# TinyMCE Ace code editor

TinyMCE plugin that uses [Ace Editor](https://ace.c9.io/) (if available) as HTML editor for improved user experience code highlighting, indentation, line numbers and more. If ACE is not available, it falls back on using textarea for code editing.

## Dependencies
- [TinyMCE](https://www.tinymce.com/) (tested with version 4)
- [jQuery](http://jquery.com/)
- [Ace Editor](https://ace.c9.io/) (optional but recommended)

## Usage
In TinyMCE init, you need to add `code_toggle` to plugins and also to the toolbar at whatever location you want the toggle button to appear.

### Example init code:
```javascript
tinymce.init({
    selector: 'textarea',
    menubar: false,
    statusbar: false,
    plugins: [
        'link textcolor colorpicker code_toggle'
    ],
    toolbar_item_size: "small",
    toolbar1: 'bold italic underline link backcolor forecolor | code_toggle',
    height : 300,
});
```
