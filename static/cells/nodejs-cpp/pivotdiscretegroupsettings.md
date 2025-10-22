##PivotDiscreteGroupSettings
Rrepsents the discrete group of pivot field
## PivotDiscreteGroupSettings class
Rrepsents the discrete group of pivot field
```javascript
class PivotDiscreteGroupSettings extends PivotFieldGroupSettings;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PivotFieldGroupSettings)](#constructor-pivotfieldgroupsettings-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [items](#items--)| CustomPiovtFieldGroupItem[] | Readonly. Gets the discrete items. |
## Methods
| Method | Description |
| --- | --- |
| [getItems()](#getItems--)| <b>@deprecated.</b> Please use the 'items' property instead. Gets the discrete items. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getType()](#getType--)| Gets the group type. |
### constructor(PivotFieldGroupSettings) {#constructor-pivotfieldgroupsettings-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: PivotFieldGroupSettings);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PivotFieldGroupSettings | The parent object. |
### items {#items--}
Readonly. Gets the discrete items.
```javascript
items : CustomPiovtFieldGroupItem[];
```
### getItems() {#getItems--}
```javascript
getItems() : CustomPiovtFieldGroupItem[];
```
**Returns**
[CustomPiovtFieldGroupItem](../custompiovtfieldgroupitem/)[]
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getType() {#getType--}
Gets the group type.
```javascript
getType() : PivotFieldGroupType;
```
**Returns**
[PivotFieldGroupType](../pivotfieldgrouptype/)
