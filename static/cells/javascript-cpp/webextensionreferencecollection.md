##WebExtensionReferenceCollection
Represents the list of web extension reference.
## WebExtensionReferenceCollection class
Represents the list of web extension reference.
```javascript
class WebExtensionReferenceCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets web extension by the specific index. |
| [add()](#add--)| Adds an empty reference of web extension. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets web extension by the specific index.
```javascript
get(index: number) : WebExtensionReference;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The web extension
### add() {#add--}
Adds an empty reference of web extension.
```javascript
add() : number;
```
