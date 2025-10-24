##PdfBookmarkEntry
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or  current instance will be hidden and children will be inserted on current level.
## PdfBookmarkEntry class
PdfBookmarkEntry is an entry in pdf bookmark. if Text property of current instance is null or "", current instance will be hidden and children will be inserted on current level.
```javascript
class PdfBookmarkEntry;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [text](#text--)| string | Title of a bookmark. |
| [destination](#destination--)| Cell | The cell to which the bookmark link. |
| [destinationName](#destinationName--)| string | Gets or sets name of destination. |
| [isOpen](#isOpen--)| boolean | When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [isCollapse](#isCollapse--)| boolean | When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
## Methods
| Method | Description |
| --- | --- |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. Title of a bookmark. |
| [setText(string)](#setText-string-)| <b>@deprecated.</b> Please use the 'text' property instead. Title of a bookmark. |
| [getDestination()](#getDestination--)| <b>@deprecated.</b> Please use the 'destination' property instead. The cell to which the bookmark link. |
| [setDestination(Cell)](#setDestination-cell-)| <b>@deprecated.</b> Please use the 'destination' property instead. The cell to which the bookmark link. |
| [getDestinationName()](#getDestinationName--)| <b>@deprecated.</b> Please use the 'destinationName' property instead. Gets or sets name of destination. |
| [setDestinationName(string)](#setDestinationName-string-)| <b>@deprecated.</b> Please use the 'destinationName' property instead. Gets or sets name of destination. |
| [isOpen()](#isOpen--)| <b>@deprecated.</b> Please use the 'isOpen' property instead. When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [setIsOpen(boolean)](#setIsOpen-boolean-)| <b>@deprecated.</b> Please use the 'isOpen' property instead. When this property is true, the bookmarkentry will expand, otherwise it will collapse. |
| [isCollapse()](#isCollapse--)| <b>@deprecated.</b> Please use the 'isCollapse' property instead. When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [setIsCollapse(boolean)](#setIsCollapse-boolean-)| <b>@deprecated.</b> Please use the 'isCollapse' property instead. When this property is true, the bookmarkentry will collapse, otherwise it will expand. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### text {#text--}
Title of a bookmark.
```javascript
text : string;
```
### destination {#destination--}
The cell to which the bookmark link.
```javascript
destination : Cell;
```
### destinationName {#destinationName--}
Gets or sets name of destination.
```javascript
destinationName : string;
```
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
### isOpen {#isOpen--}
When this property is true, the bookmarkentry will expand, otherwise it will collapse.
```javascript
isOpen : boolean;
```
### isCollapse {#isCollapse--}
When this property is true, the bookmarkentry will collapse, otherwise it will expand.
```javascript
isCollapse : boolean;
```
### getText() {#getText--}
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getDestination() {#getDestination--}
```javascript
getDestination() : Cell;
```
**Returns**
[Cell](../cell/)
### setDestination(Cell) {#setDestination-cell-}
```javascript
setDestination(value: Cell) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Cell](../cell/) | The value to set. |
### getDestinationName() {#getDestinationName--}
```javascript
getDestinationName() : string;
```
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
### setDestinationName(string) {#setDestinationName-string-}
```javascript
setDestinationName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If destination name is set, the destination will be defined as a named destination with this name.
### isOpen() {#isOpen--}
```javascript
isOpen() : boolean;
```
### setIsOpen(boolean) {#setIsOpen-boolean-}
```javascript
setIsOpen(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isCollapse() {#isCollapse--}
```javascript
isCollapse() : boolean;
```
### setIsCollapse(boolean) {#setIsCollapse-boolean-}
```javascript
setIsCollapse(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
