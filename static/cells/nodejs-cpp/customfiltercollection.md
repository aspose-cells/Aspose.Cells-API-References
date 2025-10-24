##CustomFilterCollection
Represents the custom filters.
## CustomFilterCollection class
Represents the custom filters.
```javascript
class CustomFilterCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs new instance. |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [and](#and--)| boolean | Indicates whether the two criteria have an "and" relationship. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom filter in the specific index. |
| [getAnd()](#getAnd--)| <b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship. |
| [setAnd(boolean)](#setAnd-boolean-)| <b>@deprecated.</b> Please use the 'and' property instead. Indicates whether the two criteria have an "and" relationship. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |
### constructor() {#constructor--}
Constructs new instance.
```javascript
constructor();
```
### constructor(Object) {#constructor-object-}
Constructs from an Object convertible to this.
```javascript
constructor(obj: Object);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |
### and {#and--}
Indicates whether the two criteria have an "and" relationship.
```javascript
and : boolean;
```
### get(number) {#get-number-}
Gets the custom filter in the specific index.
```javascript
get(index: number) : CustomFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[CustomFilter](../customfilter/)
### getAnd() {#getAnd--}
```javascript
getAnd() : boolean;
```
### setAnd(boolean) {#setAnd-boolean-}
```javascript
setAnd(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### toObject() {#toObject--}
Gets the Object.
```javascript
toObject() : Object;
```
