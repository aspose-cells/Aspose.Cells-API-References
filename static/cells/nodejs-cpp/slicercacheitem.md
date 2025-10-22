##SlicerCacheItem
Represent slicer data source item
## SlicerCacheItem class
Represent slicer data source item
```javascript
class SlicerCacheItem;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [selected](#selected--)| boolean | Specifies whether the SlicerItem is selected or not. |
| [value](#value--)| string | Readonly. Returns the label text for the slicer item. Read-only. |
## Methods
| Method | Description |
| --- | --- |
| [getSelected()](#getSelected--)| <b>@deprecated.</b> Please use the 'selected' property instead. Specifies whether the SlicerItem is selected or not. |
| [setSelected(boolean)](#setSelected-boolean-)| <b>@deprecated.</b> Please use the 'selected' property instead. Specifies whether the SlicerItem is selected or not. |
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Returns the label text for the slicer item. Read-only. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### selected {#selected--}
Specifies whether the SlicerItem is selected or not.
```javascript
selected : boolean;
```
### value {#value--}
Readonly. Returns the label text for the slicer item. Read-only.
```javascript
value : string;
```
### getSelected() {#getSelected--}
```javascript
getSelected() : boolean;
```
### setSelected(boolean) {#setSelected-boolean-}
```javascript
setSelected(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getValue() {#getValue--}
```javascript
getValue() : string;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
