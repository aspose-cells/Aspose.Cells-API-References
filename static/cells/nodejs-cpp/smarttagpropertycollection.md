##SmartTagPropertyCollection
Represents all properties of cell smart tag.
## SmartTagPropertyCollection class
Represents all properties of cell smart tag.
```javascript
class SmartTagPropertyCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTagProperty](../smarttagproperty/) object. |
| [get(string)](#get-string-)| Gets a [SmartTagProperty](../smarttagproperty/) object by the name of the property. |
| [add(string, string)](#add-string-string-)| Adds a property of cell's smart tag. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets a [SmartTagProperty](../smarttagproperty/) object.
```javascript
get(index: number) : SmartTagProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |
**Returns**
Returns a [SmartTagProperty](../smarttagproperty/) object.
### get(string) {#get-string-}
Gets a [SmartTagProperty](../smarttagproperty/) object by the name of the property.
```javascript
get(name: string) : SmartTagProperty;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property. |
**Returns**
Returns a [SmartTagProperty](../smarttagproperty/) object.
### add(string, string) {#add-string-string-}
Adds a property of cell's smart tag.
```javascript
add(name: string, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the property |
| value | string | The value of the property. |
**Returns**
return [SmartTagProperty](../smarttagproperty/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
