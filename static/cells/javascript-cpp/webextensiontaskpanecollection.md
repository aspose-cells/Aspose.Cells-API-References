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
