##DataSorterKey
Represents the key of the data sorter.
## DataSorterKey class
Represents the key of the data sorter.
```javascript
class DataSorterKey;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [order](#order--)| SortOrder | Readonly. Indicates the order of sorting. |
| [index](#index--)| number | Readonly. Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [type](#type--)| SortOnType | Readonly. Represents the type of sorting. |
| [iconSetType](#iconSetType--)| IconSetType | Readonly. Represents the icon set type. |
| [iconId](#iconId--)| number | Readonly. Represents the id of the icon set type. |
| [color](#color--)| Color | Readonly. Gets the sorted color. |
## Methods
| Method | Description |
| --- | --- |
| [getOrder()](#getOrder--)| <b>@deprecated.</b> Please use the 'order' property instead. Indicates the order of sorting. |
| [getIndex()](#getIndex--)| <b>@deprecated.</b> Please use the 'index' property instead. Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Represents the type of sorting. |
| [getIconSetType()](#getIconSetType--)| <b>@deprecated.</b> Please use the 'iconSetType' property instead. Represents the icon set type. |
| [getIconId()](#getIconId--)| <b>@deprecated.</b> Please use the 'iconId' property instead. Represents the id of the icon set type. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets the sorted color. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### order {#order--}
Readonly. Indicates the order of sorting.
```javascript
order : SortOrder;
```
### index {#index--}
Readonly. Gets the sorted column index(absolute position, column A is 0, B is 1, ...).
```javascript
index : number;
```
### type {#type--}
Readonly. Represents the type of sorting.
```javascript
type : SortOnType;
```
### iconSetType {#iconSetType--}
Readonly. Represents the icon set type.
```javascript
iconSetType : IconSetType;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### iconId {#iconId--}
Readonly. Represents the id of the icon set type.
```javascript
iconId : number;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### color {#color--}
Readonly. Gets the sorted color.
```javascript
color : Color;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.CellColor](../sortontype.cellcolor/) or [SortOnType.FontColor](../sortontype.fontcolor/).
### getOrder() {#getOrder--}
```javascript
getOrder() : SortOrder;
```
**Returns**
[SortOrder](../sortorder/)
### getIndex() {#getIndex--}
```javascript
getIndex() : number;
```
### getType() {#getType--}
```javascript
getType() : SortOnType;
```
**Returns**
[SortOnType](../sortontype/)
### getIconSetType() {#getIconSetType--}
```javascript
getIconSetType() : IconSetType;
```
**Returns**
[IconSetType](../iconsettype/)
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### getIconId() {#getIconId--}
```javascript
getIconId() : number;
```
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.Icon](../sortontype.icon/).
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
**Remarks**
Only takes effect when [Type](../type/) is [SortOnType.CellColor](../sortontype.cellcolor/) or [SortOnType.FontColor](../sortontype.fontcolor/).
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
