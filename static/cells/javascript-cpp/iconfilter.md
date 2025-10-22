##IconFilter
Represents icon filter.
## IconFilter class
Represents icon filter.
```javascript
class IconFilter;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(VObject)](#constructor-vobject-)| Constructs from a VObject convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [iconSetType](#iconSetType--)| IconSetType | Gets and sets which icon set is used in the filter criteria. |
| [iconId](#iconId--)| number | Gets and sets Zero-based index of an icon in an icon set. |
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
### iconSetType {#iconSetType--}
Gets and sets which icon set is used in the filter criteria.
```javascript
iconSetType : IconSetType;
```
### iconId {#iconId--}
Gets and sets Zero-based index of an icon in an icon set.
```javascript
iconId : number;
```
### toVObject() {#toVObject--}
Gets the VObject.
```javascript
toVObject() : VObject;
```
