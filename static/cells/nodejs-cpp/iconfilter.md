##IconFilter
Represents icon filter.
## IconFilter class
Represents icon filter.
```javascript
class IconFilter;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Object)](#constructor-object-)| Constructs from an Object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [iconSetType](#iconSetType--)| IconSetType | Gets and sets which icon set is used in the filter criteria. |
| [iconId](#iconId--)| number | Gets and sets Zero-based index of an icon in an icon set. |
## Methods
| Method | Description |
| --- | --- |
| [getIconSetType()](#getIconSetType--)| <b>@deprecated.</b> Please use the 'iconSetType' property instead. Gets and sets which icon set is used in the filter criteria. |
| [setIconSetType(IconSetType)](#setIconSetType-iconsettype-)| <b>@deprecated.</b> Please use the 'iconSetType' property instead. Gets and sets which icon set is used in the filter criteria. |
| [getIconId()](#getIconId--)| <b>@deprecated.</b> Please use the 'iconId' property instead. Gets and sets Zero-based index of an icon in an icon set. |
| [setIconId(number)](#setIconId-number-)| <b>@deprecated.</b> Please use the 'iconId' property instead. Gets and sets Zero-based index of an icon in an icon set. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [toObject()](#toObject--)| Gets the Object. |
### constructor(Object) {#constructor-object-}
Constructs from an Object convertible to this.
```javascript
constructor(obj: Object);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The object. |
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
### getIconSetType() {#getIconSetType--}
```javascript
getIconSetType() : IconSetType;
```
**Returns**
[IconSetType](../iconsettype/)
### setIconSetType(IconSetType) {#setIconSetType-iconsettype-}
```javascript
setIconSetType(value: IconSetType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IconSetType](../iconsettype/) | The value to set. |
### getIconId() {#getIconId--}
```javascript
getIconId() : number;
```
### setIconId(number) {#setIconId-number-}
```javascript
setIconId(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
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
