##MultipleFilterCollection
Represents the multiple filter collection.
## MultipleFilterCollection class
Represents the multiple filter collection.
```javascript
class MultipleFilterCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs one new instance. |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [matchBlank](#matchBlank--)| boolean | Indicates whether to filter by blank. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| DateTimeGroupItem or a simple object. |
| [add(string)](#add-string-)| Adds string filter. |
| [toVObject()](#toVObject--)| Gets the VObject. |
### constructor() {#constructor--}
Constructs one new instance.
```javascript
constructor();
```
### constructor(VObject) {#constructor-vobject-}
Constructs from a VObject convertible to this.
```javascript
constructor(vobj: VObject);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |
### matchBlank {#matchBlank--}
Indicates whether to filter by blank.
```javascript
matchBlank : boolean;
```
### get(number) {#get-number-}
DateTimeGroupItem or a simple object.
```javascript
get(index: number) : VObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
### add(string) {#add-string-}
Adds string filter.
```javascript
add(filter: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| filter | string | The filter data. |
### toVObject() {#toVObject--}
Gets the VObject.
```javascript
toVObject() : VObject;
```
