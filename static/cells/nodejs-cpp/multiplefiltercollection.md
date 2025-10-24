##MultipleFilterCollection
Represents the multiple filter collection.
## MultipleFilterCollection class
Represents the multiple filter collection.
```javascript
class MultipleFilterCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs one new instance. |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [matchBlank](#matchBlank--)| boolean | Indicates whether to filter by blank. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| DateTimeGroupItem or a simple object. |
| [getMatchBlank()](#getMatchBlank--)| <b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank. |
| [setMatchBlank(boolean)](#setMatchBlank-boolean-)| <b>@deprecated.</b> Please use the 'matchBlank' property instead. Indicates whether to filter by blank. |
| [add(string)](#add-string-)| Adds string filter. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |
### constructor() {#constructor--}
Constructs one new instance.
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
### matchBlank {#matchBlank--}
Indicates whether to filter by blank.
```javascript
matchBlank : boolean;
```
### get(number) {#get-number-}
DateTimeGroupItem or a simple object.
```javascript
get(index: number) : Object;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
### getMatchBlank() {#getMatchBlank--}
```javascript
getMatchBlank() : boolean;
```
### setMatchBlank(boolean) {#setMatchBlank-boolean-}
```javascript
setMatchBlank(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### add(string) {#add-string-}
Adds string filter.
```javascript
add(filter: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | string | The filter data. |
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
