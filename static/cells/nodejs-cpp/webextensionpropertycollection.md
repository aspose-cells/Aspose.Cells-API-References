##WebExtensionPropertyCollection
Represents the list of web extension properties.
## WebExtensionPropertyCollection class
Represents the list of web extension properties.
```javascript
class WebExtensionPropertyCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the property of web extension by the index. |
| [get(string)](#get-string-)| Gets the property of web extension. |
| [add(string, string)](#add-string-string-)| Adds web extension property. |
| [removeAt(string)](#removeAt-string-)| Remove the property by the name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets the property of web extension by the index.
```javascript
get(index: number) : WebExtensionProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The property of web extension.
### get(string) {#get-string-}
Gets the property of web extension.
```javascript
get(name: string) : WebExtensionProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of property. |
**Returns**
The property of web extension.
### add(string, string) {#add-string-string-}
Adds web extension property.
```javascript
add(name: string, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of property. |
| value | string | The value of property. |
**Returns**
The index of added property.
### removeAt(string) {#removeAt-string-}
Remove the property by the name.
```javascript
removeAt(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
