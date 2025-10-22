##PivotTableFormat
Represents the format defined in the PivotTable.
## PivotTableFormat class
Represents the format defined in the PivotTable.
```javascript
class PivotTableFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pivotArea](#pivotArea--)| PivotArea | Readonly. Gets the pivot area. |
## Methods
| Method | Description |
| --- | --- |
| [getPivotArea()](#getPivotArea--)| <b>@deprecated.</b> Please use the 'pivotArea' property instead. Gets the pivot area. |
| [getStyle()](#getStyle--)| Gets the formatted style. |
| [setStyle(Style)](#setStyle-style-)| Sets the style of the pivot area. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### pivotArea {#pivotArea--}
Readonly. Gets the pivot area.
```javascript
pivotArea : PivotArea;
```
### getPivotArea() {#getPivotArea--}
```javascript
getPivotArea() : PivotArea;
```
**Returns**
[PivotArea](../pivotarea/)
### getStyle() {#getStyle--}
Gets the formatted style.
```javascript
getStyle() : Style;
```
**Returns**
[Style](../style/)
### setStyle(Style) {#setStyle-style-}
Sets the style of the pivot area.
```javascript
setStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) |  |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
