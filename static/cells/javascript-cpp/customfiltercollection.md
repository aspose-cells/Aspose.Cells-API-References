##CustomFilterCollection
Represents the custom filters.
## CustomFilterCollection class
Represents the custom filters.
```javascript
class CustomFilterCollection;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Constructs new instance. |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [and](#and--)| boolean | Indicates whether the two criteria have an "and" relationship. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the custom filter in the specific index. |
| [toVObject()](#toVObject--)| Gets the VObject. |
### constructor() {#constructor--}
Constructs new instance.
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
### toVObject() {#toVObject--}
Gets the VObject.
```javascript
toVObject() : VObject;
```
