# Google Place Picker
Google's Place Picker library for web like Android and iOS

<img src="https://raw.githubusercontent.com/bewithdhanu/Google-Place-Picker/master/PlacePicker.png" width="150" height="150"></img>

### Features

- No need to write a lots of code for Google Place Picker
- Supports with jquery(3.0 or 3+), bootstrap(3.0 or 3+) and fontawesome libraries
- easily to use this PlacePicker with simple steps
- You can pick location from map or you can search location
- Compatible with all  browsers (IE8+), and mobiles;
- Support with Google API Key;
- displays a button an the end of yout input, by clicking button you will see popup screen

### How it works:
1. Click the Map Icon inside the input field.
2. Type an address in the Place Picker Popup.
3. Click the Select button to insert the Place into the input field.

<a href="https://paypal.me/bewithdhanu" target="_blank" title="Buy me a coffe"><img src="https://raw.githubusercontent.com/bewithdhanu/Google-Place-Picker/master/buy-me-a-coffee.png" height="180"></img></a>

### Usage

#### Include the needed jQuery, Bootstrap and FontAwesome on the page.
```html
<link rel="stylesheet" href="/path/to/bootstrap.min.css">
<link rel="stylesheet" href="/path/to/font-awesome.min.css">
<script src="/path/to/jquery.min.js"></script>
<script src="/path/to/bootstrap.min.js"></script>
<script src="PlacePicker.js"></script>
```
#### Create an input field for the Place Picker.

```html
<input type="email" id="input_location" class="form-control" placeholder="Address"  autofocus>
```

#### And then below Javascript snippet 

```javascript
$(document).ready(function(){
	$("#input_location").PlacePicker({
		title:"Popup Title Here",
		key:"YOUR_API_KEY",
		btnClass:"btn btn-secondary btn-sm",
		center: {lat: 17.6868, lng: 83.2185},
		success:function(data,address){
			//data contains address elements 
			//data['location'] contains Latitude and Longitude information
			//address conatins you searched text
			//Your logic here
		}
	});
});

```


#### Images

Image:

![](https://raw.githubusercontent.com/bewithdhanu/Google-Place-Picker/master/Screenshot%202019-04-03%20at%204.43.24%20PM.png)

> How map button lokks like in HTML Page

![](https://raw.githubusercontent.com/bewithdhanu/Google-Place-Picker/master/Screenshot%202019-04-03%20at%204.44.31%20PM.png)

> How map button lokks like in HTML Page

### Required Plugins
- jQuery
- Bootstrap (css & js)
- Font Awesone

                    
#### Tables
                    

#### Functions
| Function name | Description                    |
| ------------- | ------------------------------ |
| `success()`      | with 2 parameters, one is for address components, anothe ron eis for searched address.       |
#### Parameters
| Parameter name | Description                    |
| ------------- | ------------------------------ |
| key      | Your Google API Key |
| title      | Popup Title |
| center      | Default map location |
| btnClass      | Default btn class which comes on hover |
| zoom      | Set zoom level. Default: 18 |

----

### End
