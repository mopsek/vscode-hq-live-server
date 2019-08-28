# HQ Live Server

💫 **One tool to rule them all**

[![VSCode Marketplace](https://img.shields.io/vscode-marketplace/v/hqjs.hq-live-server.svg?style=flat-square&label=vscode%20marketplace)](https://marketplace.visualstudio.com/items?itemName=hqjs.hq-live-server) [![Total Installs](https://img.shields.io/vscode-marketplace/d/hqjs.hq-live-server.svg?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=hqjs.hq-live-server) [![Avarage Rating](https://img.shields.io/vscode-marketplace/r/hqjs.hq-live-server.svg?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=hqjs.hq-live-server)  
[![Travis branch](https://img.shields.io/travis/hqjs/vscode-hq-live-server/master.svg?style=flat-square&label=travis%20branch)](https://travis-ci.org/hqjs/vscode-hq-live-server) [![Appveyor branch](https://img.shields.io/appveyor/ci/hqjs/vscode-hq-live-server.svg?style=flat-square&label=appveyor%20branch)](https://ci.appveyor.com/project/hqjs/vscode-hq-live-server) [![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/hqjs/vscode-hq-live-server/)
<br>

**Launch a local development server with live reload feature for static & dynamic pages.**
<br>

![Live Server Demo VSCode](./images/screen/hq-go-live.gif)

## Shortcuts to Start/Stop Server

1. Open a project and click to `Go Live` from the status bar to turn the server on/off. 
![Go Live Control Preview](./images/screen/hq-statusbar.png)

2. Right click on a project file from Explorer Window and click on `Serve project`.
![Explorer Window Control](./images/screen/hq-explorer-menu.png).

3. Open a project file and right-click on the editor and  click on `Serve project`.
![Edit Menu Option Preview](./images/screen/hq-editor-menu.png)

4. Hit `(alt+H, alt+O)` to Open the Server and `(alt+H, alt+C)` to Stop the server (You can change the shortcut form keybinding). *[On MAC, `cmd+H, cmd+O` and `cmd+H, cmd+C`]*

5. Open the Command Pallete by pressing `F1` or `ctrl+shift+P` and type `HQ Live Server: Serve project ` to start a server or type `HQ Live Server: Stop Server` to stop a server.


## Features
* A Quick [Development Live Server](https://hqjs.org) with live browser reload.
* Quick start with any framework: Polymer, Svelte, Vue, React, Angular or plain js.
* No configuration is required.
* Start or Stop server by a single click from status bar.
* Hot Key control.
* Customizable preferred Port Number and/or default browser.
* Support for any browser _(Eg: Firefox Nightly)_ using advance Command Line.
* Support for Chrome Debugging Attachment (_[More Info](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)_).
* Remote Connect through WLAN (E.g.: Connect with mobile)
* Multi-root workspace supported.

## Installation
Open VSCode and type `ctrl+P`, type `ext install hqjs.hq-live-server`.

## FAQs
* How to access the server from Mobile?

  After you pressed `Go Live` button server address will appear
  ![Server Running Preview](./images/screen/hq-running.png)
  follow this address on your mobile device within your local network.

* Are Multi-root workspaces supported?

  Yes, you can run separate server instance for every project in your workspace.

* Do I need to configure webpack or babel to start development?
  
  No, you can press `Go Live` button and start development immediatly. Extension will take care of everything else.

## Settings
* **`hqServer.defaultPort`:** Preferred Port Number for your Live Server.
    *  _Default value is `8080`._

    <hr>

* **`hqServer.showOnStatusbar`:** Display `Go Live` button on the statusbar.
    *  _Default value is `true`._

    <hr>

* **`hqServer.browser.useBuiltinBrowser`:** Open in [Browser Preview](https://marketplace.visualstudio.com/items?itemName=auchenberg.vscode-browser-preview) extension inside VS Code, instead of default browser.
    
    *  _Default value is `false`.

    <hr>

* **`hqServer.browser.preferredBrowser`:** To change your system's default browser.
    * _Default value is `""`. (It will open your system's default browser.)_
    * *Available Options :*
        * chrome
        * chrome:PrivateMode
        * firefox
        * firefox:PrivateMode
        * safari
        * microsoft-edge
        * blisk

    _Not enough? need more? open an/a issue/pull request on github. For now, use `hqServer.browser.browserCmdLine` settings (see below)._
    
    <hr>

* **`hqServer.browser.browserCmdLine`:**  To set your any favorite browser (Eg: Chrome Canary, Firefox Nightly) using advance Command Line. _(You can specify full path of your favorite custom browser)_.

    * _This setting will override `Preferred Browser` and `Attach Chrome Debugger` settings._
    * _Default Value is `""`_ 
    * _Examples:_
        * _chrome --incognito --headless --remote-debugging-port=9222_
        * _C:\\Program Files\\Firefox Developer Edition\\firefox.exe --private-window_
    
    <hr>

* **`hqServer.browser.attachChromeDebugger`:** To Enable Chrome Debugging Attachment to Live Server.
    * _**NOTE**: You must have to install [ `Debugger for Chrome.`](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome)_
    
    * _If the value is `true`, Start Live Server and select 'Attach to Chrome' from Debug Window to start debugging. [`Debugger for Chrome`](https://marketplace.visualstudio.com/items?itemName=msjsdiag.debugger-for-chrome) Extension will inject debugging feature into running instance of browser window._
   
    *  _Default value is `false`._

    <hr>


## LICENSE
This extension is licensed under the [MIT License](LICENSE)
