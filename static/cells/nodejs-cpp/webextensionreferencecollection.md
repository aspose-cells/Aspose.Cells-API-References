##WebExtensionReferenceCollection
Represents the list of web extension reference.
## WebExtensionReferenceCollection class
Represents the list of web extension reference.
```javascript
class WebExtensionReferenceCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets web extension by the specific index. |
| [add()](#add--)| Adds an empty reference of web extension. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
