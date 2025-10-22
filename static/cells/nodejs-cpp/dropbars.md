##DropBars
Represents the updown bars in a chart.
## DropBars class
Represents the up/down bars in a chart.
```javascript
class DropBars;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [border](#border--)| Line | Readonly. Gets the border [Line](../line/). |
| [area](#area--)| Area | Readonly. Gets the [Area](../area/). |
## Methods
| Method | Description |
| --- | --- |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Gets the border [Line](../line/). |
| [getArea()](#getArea--)| <b>@deprecated.</b> Please use the 'area' property instead. Gets the [Area](../area/). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### border {#border--}
Readonly. Gets the border [Line](../line/).
```javascript
border : Line;
```
### area {#area--}
Readonly. Gets the [Area](../area/).
```javascript
area : Area;
```
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### getArea() {#getArea--}
```javascript
getArea() : Area;
```
**Returns**
[Area](../area/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
