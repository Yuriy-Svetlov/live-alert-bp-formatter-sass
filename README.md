# Live Alert BP Formatter SASS

The SASS message formatter for [live-alert-bp](https://github.com/Yuriy-Svetlov/live-alert-bp)


##  Install
```shell
npm i live-alert-bp-formatter-sass --save-dev
```

## How to use

```javascript
  const formatterSASS = require("live-alert-bp-formatter-sass");

  liveAlert.open(
    formatterSASS(MessagesSASS)
  );
```

## Examples how to use

[Examples](https://github.com/Yuriy-Svetlov/live-alert-bp#examples)

## API

```javascript
const formatterSASS = require("live-alert-bp-formatter-sass");

formatterSASS(messages, user_style)
```

* return: formatted messages for [live-alert-bp](https://github.com/Yuriy-Svetlov/live-alert-bp)

#### messages
* Type: `Array`

SASS messages

#### user_style
* Type: `ObjectJSON`

Set custom style messages

Exmaple:
```javascript
  const style = {};	

  style.label = {
	error: { backgroundColor: '#ff0000', color: '#ffffff' },
	warning: { backgroundColor: 'yellow', color: '#000000' },
	info: { backgroundColor: '#90ee90', color: '#000000' }
  };

  style.file = 'color: #90ee90 !important; text-decoration: underline !important;';
	
  style.line = {
	field: 'color: #aaaaaa !important; padding-left: 7px !important;', 
	message: 'color: #ffffff !important; padding-left: 3px !important;'
  };
	
  style.column = {
	field: 'color: #aaaaaa !important; padding-left: 7px !important;', 
	message: 'color: #ffffff !important; padding-left: 3px !important;'
  };

  style.evidence = {
	field: 'color: #aaaaaa !important; display: block !important; padding-bottom: 8px !important;', 
	message: 'box-sizing: border-box !important; width: 100% !important; overflow-x: auto !important; color: #ffffff !important; display: inline-block !important; border: dashed 1px #b9b9b9 !important; padding: 20px !important;'
  };

  style.reason = {
	field: 'color: #aaaaaa !important; display: block !important;  padding-top: 3px !important;', 
		message: 'color: #ffffff !important;'
  };	
```
