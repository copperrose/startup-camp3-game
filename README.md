# Startup Camp3 - HTML5 Game Development

## List for development environment

- [Sublime text](http://www.sublimetext.com/3)
	- [Package Control](https://sublime.wbond.net/)
	- [EditorConfig](http://editorconfig.org/)
	- [Emmet](http://emmet.io)
- [Github](https://github.com)
- [NodeJS](http://nodejs.org/)
	- [npm](https://npmjs.org/)
	- [Express](http://expressjs.com)
- [Bower](http://bower.io)
	- [Bootstrap](http://getbootstrap.com)
	- [jQuery](http://jquery.com)
	-	[jQuery-tmpl](https://github.com/BorisMoore/jquery-tmpl)

## Note

### Set Windows to show invalid files and file extension name

### Install Package Control on Sublime Text 3 (Ctrl + `)
```
import urllib.request,os; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); open(os.path.join(ipp, pf), 'wb').write(urllib.request.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ','%20')).read())
```

### Install editorconfig
```
Ctrl + Shift + P
type 'Install Package'
type 'Editorconfig'
```

#### .editorconfig
```
; top-most EditorConfig file
root = true

[*]
indent_style = space
indent_size = 4
end_of_line = lf
charset = utf-8
3insert_final_newline = true
trim_trailing_whitespace = true
```

### Install Emmet
```
Ctrl + Shift + P
type 'Install Package'
type 'Emmet'
```

### Install NodeJS Web Server (ExpressJS)
```
$ npm install -g express
```

### Install Bower (front-end package manager)
```
$ npm install -g bower
```
bower init
bower install bootstrap --save
bower install query --save
bower install jquery-tmpl --save
bower install
```

## Stage 1

Refactor 912492d7adb5c4368c1496af87a632f694f30b62

- Move JavaScript code to main.chat.js
- Using JavaScript closure (module)
- Using yepnope loader

## Stage 2

Mapping view and data

- Using key-value pairs (ViewModel): use JSON to present key-value data
- Using Backbone (fully application framework) for applying ViewModel, or
- Simple template library (eg. [jquery template](https://github.com/BorisMoore/jquery-tmpl))
- UI made easy: use Bootstrap CSS framework

## Stage 3

Application

- Use Bootstrap navbars
- Responsive design by Bootstrap

## Stage 4

Send data

- Use WebSocket send()
- Connect Open API: AJAX and RESTful
- Not use AJAX method: if so, either jQuery way or Backbone way is good
- Not use RESTful API: refactor URL query string to REST spec

## Stage 5

Going mobile

- Use PhoneGap: build.phonegap.com or Eclipse+PhoneGap
- Use viewport
- Use Mixins (LESS) to set media query of 'screen' height

## Stage 6

Using PhoneGap APIs

- Camera web app

## Stage 7

Enter Nodejs: Developing Web service

- Create a Web server
- Handling URL routing
- Create WebSocket server
- Handling requests

## Stage 8

Using package.json

- for releasing software

## Final Stage

- Use jQuery AJAX and JSON data instead of query string
- use preventDefault()
- use jQuery UI Touch Punch ('touchmove' event)
- Try Express.js and understanding RESTful
