##WebExtensionBindingCollection
Represents the list of binding relationships between an Office Addin and the data in the document.
## WebExtensionBindingCollection class
Represents the list of binding relationships between an Office Add-in and the data in the document.
```javascript
class WebExtensionBindingCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets web extension binding relationship by the specific index. |
| [add()](#add--)| Adds an a binding relationship between an Office Add-in and the data in the document. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets web extension binding relationship by the specific index.
```javascript
get(index: number) : WebExtensionBinding;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The  web extension binding relationship
### add() {#add--}
Adds an a binding relationship between an Office Add-in and the data in the document.
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
