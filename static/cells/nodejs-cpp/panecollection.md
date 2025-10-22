##PaneCollection
Represents all Pane objects shown in the specified window.
## PaneCollection class
Represents all Pane objects shown in the specified window.
```javascript
class PaneCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [firstVisibleRowOfBottomPane](#firstVisibleRowOfBottomPane--)| number | Gets and sets the first visible row of the bottom pane. |
| [firstVisibleColumnOfRightPane](#firstVisibleColumnOfRightPane--)| number | Gets and sets the first visible column of the right pane. |
| [acitvePaneType](#acitvePaneType--)| RectangleAlignmentType | Gets and sets the active pane. |
## Methods
| Method | Description |
| --- | --- |
| [getFirstVisibleRowOfBottomPane()](#getFirstVisibleRowOfBottomPane--)| <b>@deprecated.</b> Please use the 'firstVisibleRowOfBottomPane' property instead. Gets and sets the first visible row of the bottom pane. |
| [setFirstVisibleRowOfBottomPane(number)](#setFirstVisibleRowOfBottomPane-number-)| <b>@deprecated.</b> Please use the 'firstVisibleRowOfBottomPane' property instead. Gets and sets the first visible row of the bottom pane. |
| [getFirstVisibleColumnOfRightPane()](#getFirstVisibleColumnOfRightPane--)| <b>@deprecated.</b> Please use the 'firstVisibleColumnOfRightPane' property instead. Gets and sets the first visible column of the right pane. |
| [setFirstVisibleColumnOfRightPane(number)](#setFirstVisibleColumnOfRightPane-number-)| <b>@deprecated.</b> Please use the 'firstVisibleColumnOfRightPane' property instead. Gets and sets the first visible column of the right pane. |
| [getAcitvePaneType()](#getAcitvePaneType--)| <b>@deprecated.</b> Please use the 'acitvePaneType' property instead. Gets and sets the active pane. |
| [setAcitvePaneType(RectangleAlignmentType)](#setAcitvePaneType-rectanglealignmenttype-)| <b>@deprecated.</b> Please use the 'acitvePaneType' property instead. Gets and sets the active pane. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### firstVisibleRowOfBottomPane {#firstVisibleRowOfBottomPane--}
Gets and sets the first visible row of the bottom pane.
```javascript
firstVisibleRowOfBottomPane : number;
```
### firstVisibleColumnOfRightPane {#firstVisibleColumnOfRightPane--}
Gets and sets the first visible column of the right pane.
```javascript
firstVisibleColumnOfRightPane : number;
```
### acitvePaneType {#acitvePaneType--}
Gets and sets the active pane.
```javascript
acitvePaneType : RectangleAlignmentType;
```
### getFirstVisibleRowOfBottomPane() {#getFirstVisibleRowOfBottomPane--}
```javascript
getFirstVisibleRowOfBottomPane() : number;
```
### setFirstVisibleRowOfBottomPane(number) {#setFirstVisibleRowOfBottomPane-number-}
```javascript
setFirstVisibleRowOfBottomPane(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getFirstVisibleColumnOfRightPane() {#getFirstVisibleColumnOfRightPane--}
```javascript
getFirstVisibleColumnOfRightPane() : number;
```
### setFirstVisibleColumnOfRightPane(number) {#setFirstVisibleColumnOfRightPane-number-}
```javascript
setFirstVisibleColumnOfRightPane(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAcitvePaneType() {#getAcitvePaneType--}
```javascript
getAcitvePaneType() : RectangleAlignmentType;
```
**Returns**
[RectangleAlignmentType](../rectanglealignmenttype/)
### setAcitvePaneType(RectangleAlignmentType) {#setAcitvePaneType-rectanglealignmenttype-}
```javascript
setAcitvePaneType(value: RectangleAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RectangleAlignmentType](../rectanglealignmenttype/) | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
