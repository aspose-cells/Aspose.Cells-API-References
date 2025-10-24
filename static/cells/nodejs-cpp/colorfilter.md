##ColorFilter
Represents filtering the range by color.
## ColorFilter class
Represents filtering the range by color.
```javascript
class ColorFilter;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [filterByFillColor](#filterByFillColor--)| boolean | Whether filter by the cell's fill color. |
## Methods
| Method | Description |
| --- | --- |
| [getFilterByFillColor()](#getFilterByFillColor--)| <b>@deprecated.</b> Please use the 'filterByFillColor' property instead. Whether filter by the cell's fill color. |
| [setFilterByFillColor(boolean)](#setFilterByFillColor-boolean-)| <b>@deprecated.</b> Please use the 'filterByFillColor' property instead. Whether filter by the cell's fill color. |
| [getColor(WorksheetCollection)](#getColor-worksheetcollection-)| Gets the color of this filter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |
### constructor(Object) {#constructor-object-}
Constructs from an Object convertible to this.
```javascript
constructor(obj: Object);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |
### filterByFillColor {#filterByFillColor--}
Whether filter by the cell's fill color.
```javascript
filterByFillColor : boolean;
```
**Remarks**
True: cell's fill color; False: cell's font color.
### getFilterByFillColor() {#getFilterByFillColor--}
```javascript
getFilterByFillColor() : boolean;
```
**Remarks**
True: cell's fill color; False: cell's font color.
### setFilterByFillColor(boolean) {#setFilterByFillColor-boolean-}
```javascript
setFilterByFillColor(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
True: cell's fill color; False: cell's font color.
### getColor(WorksheetCollection) {#getColor-worksheetcollection-}
Gets the color of this filter.
```javascript
getColor(sheets: WorksheetCollection) : Color;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheets | [WorksheetCollection](../worksheetcollection/) |  |
**Returns**
[Color](../color/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### toObject() {#toObject--}
Gets the Object.
```javascript
toObject() : Object;
```
