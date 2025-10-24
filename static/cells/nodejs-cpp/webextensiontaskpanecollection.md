##WebExtensionTaskPaneCollection
Represents the list of task pane.
## WebExtensionTaskPaneCollection class
Represents the list of task pane.
```javascript
class WebExtensionTaskPaneCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets task pane by the specific index. |
| [add()](#add--)| Adds task pane. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets task pane by the specific index.
```javascript
get(index: number) : WebExtensionTaskPane;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The task pane.
### add() {#add--}
Adds task pane.
```javascript
add() : number;
```
**Returns**
The index.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
