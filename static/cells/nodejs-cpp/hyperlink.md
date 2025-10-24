##Hyperlink
Encapsulates the object that represents a hyperlink.
## Hyperlink class
Encapsulates the object that represents a hyperlink.
```javascript
class Hyperlink;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Adding a new worksheet to the Workbook object
workbook.worksheets.add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Adding a hyperlink to a URL at "A1" cell
worksheet.hyperlinks.add("A1", 1, 1, "https://www.aspose.com");
//Saving the Excel file
workbook.save("output/Hyperlink.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [address](#address--)| string | Represents the address of a hyperlink. |
| [textToDisplay](#textToDisplay--)| string | Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [area](#area--)| CellArea | Readonly. Gets the range of hyperlink. |
| [screenTip](#screenTip--)| string | Returns or sets the ScreenTip text for the specified hyperlink. |
| [linkType](#linkType--)| TargetModeType | Readonly. Gets the link type. |
## Methods
| Method | Description |
| --- | --- |
| [getAddress()](#getAddress--)| <b>@deprecated.</b> Please use the 'address' property instead. Represents the address of a hyperlink. |
| [setAddress(string)](#setAddress-string-)| <b>@deprecated.</b> Please use the 'address' property instead. Represents the address of a hyperlink. |
| [getTextToDisplay()](#getTextToDisplay--)| <b>@deprecated.</b> Please use the 'textToDisplay' property instead. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [setTextToDisplay(string)](#setTextToDisplay-string-)| <b>@deprecated.</b> Please use the 'textToDisplay' property instead. Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink. |
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Gets the range of hyperlink. |
| [getScreenTip()](#getScreenTip--)| <b>@deprecated.</b> Please use the 'screenTip' property instead. Returns or sets the ScreenTip text for the specified hyperlink. |
| [setScreenTip(string)](#setScreenTip-string-)| <b>@deprecated.</b> Please use the 'screenTip' property instead. Returns or sets the ScreenTip text for the specified hyperlink. |
| [getLinkType()](#getLinkType--)| <b>@deprecated.</b> Please use the 'linkType' property instead. Gets the link type. |
| [delete()](#delete--)| Deletes this hyperlink |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### address {#address--}
Represents the address of a hyperlink.
```javascript
address : string;
```
### textToDisplay {#textToDisplay--}
Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.
```javascript
textToDisplay : string;
```
### area {#area--}
Readonly. Gets the range of hyperlink.
```javascript
area : CellArea;
```
### screenTip {#screenTip--}
Returns or sets the ScreenTip text for the specified hyperlink.
```javascript
screenTip : string;
```
### linkType {#linkType--}
Readonly. Gets the link type.
```javascript
linkType : TargetModeType;
```
### getAddress() {#getAddress--}
```javascript
getAddress() : string;
```
### setAddress(string) {#setAddress-string-}
```javascript
setAddress(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTextToDisplay() {#getTextToDisplay--}
```javascript
getTextToDisplay() : string;
```
### setTextToDisplay(string) {#setTextToDisplay-string-}
```javascript
setTextToDisplay(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getArea() {#getArea--}
```javascript
getArea() : CellArea;
```
**Returns**
[CellArea](../cellarea/)
### getScreenTip() {#getScreenTip--}
```javascript
getScreenTip() : string;
```
### setScreenTip(string) {#setScreenTip-string-}
```javascript
setScreenTip(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getLinkType() {#getLinkType--}
```javascript
getLinkType() : TargetModeType;
```
**Returns**
[TargetModeType](../targetmodetype/)
### delete() {#delete--}
Deletes this hyperlink
```javascript
delete() : void;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
