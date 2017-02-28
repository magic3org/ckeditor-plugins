# 概要(Summary)

CKEditor 4用のプラグインです。
Plugins for CKEditor 4.

# インストール(Install)
CKEditorプラグインディレクトリにディレクトリごとコピー。
Copy the plugin directory into CKEditor plugin directory.

Add configuration if the plugin needs.

## Google Maps plugin

It requires jQuery library.

```
<script src="https://code.jquery.com/jquery-1.12.4.min.js"></script>
```
Load Google Maps API.

```
<script src="https://maps.googleapis.com/maps/api/js?key=YOUR_GOOGLE_MAPS_API_KEY"></script>
```

Cofiguration sample
```
CKEDITOR.replace('editor', {
	language: 'en',
	//	language: 'ja',
	extraPlugins: 'googlemaps',
	googlemapsPlugin: {
		apiKey: "YOUR_GOOGLE_MAPS_API_KEY"
	},
	toolbar: [
		["Source"],                                  
		["Link", "Image", "Table", "HorizontalRule"],
		["Bold", "Underline", "Strike"],             
		["Googlemaps"],                                 // Google Maps plugin
	],
});
```

# 使い方(How to use)

http://doc.magic3.org/index.php?%E8%A8%AD%E5%AE%9A%E6%96%B9%E6%B3%95%2FGoogle%E3%83%9E%E3%83%83%E3%83%97
