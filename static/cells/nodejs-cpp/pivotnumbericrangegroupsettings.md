##PivotNumbericRangeGroupSettings
Represents the numberic range group of the pivot field.
## PivotNumbericRangeGroupSettings class
Represents the numberic range group of the pivot field.
```javascript
class PivotNumbericRangeGroupSettings extends PivotFieldGroupSettings;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PivotFieldGroupSettings)](#constructor-pivotfieldgroupsettings-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [start](#start--)| number | Readonly. Gets the start number of the group. |
| [end](#end--)| number | Readonly. Gets the end number of the group. |
| [interval](#interval--)| number | Readonly. Gets the interval of the group. |
## Methods
| Method | Description |
| --- | --- |
| [getStart()](#getStart--)| <b>@deprecated.</b> Please use the 'start' property instead. Gets the start number of the group. |
| [getEnd()](#getEnd--)| <b>@deprecated.</b> Please use the 'end' property instead. Gets the end number of the group. |
| [getInterval()](#getInterval--)| <b>@deprecated.</b> Please use the 'interval' property instead. Gets the interval of the group. |
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
### start {#start--}
Readonly. Gets the start number of the group.
```javascript
start : number;
```
### end {#end--}
Readonly. Gets the end number of the group.
```javascript
end : number;
```
### interval {#interval--}
Readonly. Gets the interval of the group.
```javascript
interval : number;
```
### getStart() {#getStart--}
```javascript
getStart() : number;
```
### getEnd() {#getEnd--}
```javascript
getEnd() : number;
```
### getInterval() {#getInterval--}
```javascript
getInterval() : number;
```
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
