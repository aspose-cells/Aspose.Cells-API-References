##WebExtensionCollection
Represents the list of web extension.
## WebExtensionCollection class
Represents the list of web extension.
```javascript
class WebExtensionCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets web extension by the specific index. |
| [add()](#add--)| Adds a web extension. |
| [addWebVideoPlayer(string, boolean, number, number)](#addWebVideoPlayer-string-boolean-number-number-)| Add a web video player into exel. |
| [removeAt(number)](#removeAt-number-)| Remove web extension by the index. |
### get(number) {#get-number-}
Gets web extension by the specific index.
```javascript
get(index: number) : WebExtension;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The  web extension.
### add() {#add--}
Adds a web extension.
```javascript
add() : number;
```
**Returns**
The index.
### addWebVideoPlayer(string, boolean, number, number) {#addWebVideoPlayer-string-boolean-number-number-}
Add a web video player into exel.
```javascript
addWebVideoPlayer(url: string, autoPlay: boolean, startTime: number, endTime: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| url | string |  |
| autoPlay | boolean | Indicates whether auto playing the video. |
| startTime | number | The start time in unit of seconds. |
| endTime | number | The end time in unit of seconds. |
### removeAt(number) {#removeAt-number-}
Remove web extension by the index.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
