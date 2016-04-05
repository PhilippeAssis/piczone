# PicZone
Crop, scrawls, resize, rotate and upload image. An updated fork and implementation of [andyvr/picEdit](https://github.com/andyvr/picEdit)

## Installation
###  Borwer
```bower install piczone```
### Git clone
```git clone https://github.com/PhilippeAssis/piczone```
### Download Master
[PhilippeAssis/piczone/archive/master.zip](https://github.com/PhilippeAssis/piczone/archive/master.zip)

## What's new:
### i18n
Simple internationalization system
Just add the files already created or customize
#### Adding i18n files
Add the script language to be defined

```html 
<script type="text/javascript" src="i18n/en.i18n.picedit.js"></script>
```

Set the language in the 'lang' option 
```javascript 
lang: 'en'
```

### Custom Internationalization
Set
```javascript 
var PICZONE_I18N = {
    'en' : {
        webcamError : "No video source detected! Please allow camera access!",
        webRTCError: "Sorry, your browser doesn't support WebRTC!",
        info: "or copy/paste image here",
        imageEmpty: "Open an image or use your camera to make a photo!",
        formDataError: "Sorry, the FormData API is not supported!",
        dataSubmitSuccess : "Data successfully submitted!",
        dataSubmitError : "Server did not accept data!"
    }
}
```
### Fixed Tools
To display the tools in the standard for image top and no hidden them 
```javascript 
activeNavBox: true
```

## Usage
Include...
```javascript
 $(function () {
        $('input[type=file]').picZone({
            activeNavBox: true, //new option
            lang: 'en' //new option
        });
    });
```

More information on [andyvr/picEdit](https://github.com/andyvr/picEdit)