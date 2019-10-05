# Ease - Low contrast, light theme, very easy on the eyes

## Supported Languages 
Polished support for ES6 (JavaScript), HTML, CSS, SCSS, Markdown, JSON. General support for most other languages, based on the colors used for JavaScript.

!["Full Editor Screenshot"][6]

## About **Ease**
**Ease** is a sister theme to [Daobeam][1], and shares it's goal of being a theme that is not trying to be cool, but is comfortable for the eyes and helps you code. I am open to pull requests and constructive feedback. If you like **Ease**, please review it.

## User Settings Recommendations
VS Code user settings has properties to increase the font-size of the source code (`editor.fontSize`), the terminal (`terminal.integrated.fontSize`), but *not* the editor sidebar. Here is a workaround for this limitation: Increase the overall font-size of everything using `window.zoomLevel`, and then slightly *decrease* the `editor.fontSize` and `terminal.integrated.fontSize` to compensate for increasing `window.zoomLevel`:

```
{
    "workbench.colorTheme": "Ease",
    "editor.fontFamily": "Consolas",
    "editor.wordWrap": "on",
    "files.autoSave": "onFocusChange",
    
    //BEGIN these settings work in tandem ~~~~~~~~
    "window.zoomLevel": 0.7, // 0.7<-- keep this value in a comment, because it will be overwritten on ctrl + 0, ctrl + +, or ctrl + -.
    "editor.fontSize": 16, // smaller than I would want it if window.zoomLevel was 0
    "terminal.integrated.fontSize": 15, //smaller than I would want it if window.zoomLevel was 0
    //END these settings work in tandem ~~~~~~~~    
}
```
## Pay it Forward at World Community Grid
Please join the [Daobeam World Community Grid team](https://join.worldcommunitygrid.org?teamId=RF7TGV6H72). Just sign up, download the software, and start crunching.

## License
GNU General Public License v3.0

## Enjoy **Ease**!

[1]:https://marketplace.visualstudio.com/items?itemName=mike-flanigan.Daobeam

[6]:https://raw.githubusercontent.com/76784/Ease/master/screenshots/full-editor.png

[7]:https://join.worldcommunitygrid.org?teamId=RF7TGV6H72
