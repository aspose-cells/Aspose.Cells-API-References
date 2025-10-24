##Top10Filter
Represents the top 10 filter.
## Top10Filter class
Represents the top 10 filter.
```javascript
class Top10Filter;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isTop](#isTop--)| boolean | Indicates whether it's top filter. |
| [isPercent](#isPercent--)| boolean | Indicates whether the items is percent. |
| [items](#items--)| number | Gets and sets the items of the filter. |
| [criteria](#criteria--)| VObject |  |
## Methods
| Method | Description |
| --- | --- |
| [toVObject()](#toVObject--)| Gets the VObject. |
### constructor(VObject) {#constructor-vobject-}
Constructs from a VObject convertible to this.
```javascript
constructor(vobj: VObject);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| vobj | VObject | The vobject. |
### isTop {#isTop--}
Indicates whether it's top filter.
```javascript
isTop : boolean;
```
### isPercent {#isPercent--}
Indicates whether the items is percent.
```javascript
isPercent : boolean;
```
### items {#items--}
Gets and sets the items of the filter.
```javascript
items : number;
```
### criteria {#criteria--}
```javascript
criteria : VObject;
```
### toVObject() {#toVObject--}
Gets the VObject.
```javascript
toVObject() : VObject;
```
