##PivotDateTimeRangeGroupSettings
Represents the field grouped by date time range.
## PivotDateTimeRangeGroupSettings class
Represents the field grouped by date time range.
```javascript
class PivotDateTimeRangeGroupSettings extends PivotFieldGroupSettings;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(PivotFieldGroupSettings)](#constructor-pivotfieldgroupsettings-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [start](#start--)| Date | Readonly. Gets the start date time of the group. |
| [end](#end--)| Date | Readonly. Gets the end date time of the group. |
| [interval](#interval--)| number | Readonly. Gets the internal of the group. |
| [groupByTypes](#groupByTypes--)| PivotGroupByType[] | Readonly. Gets the types of grouping by date time. |
## Methods
| Method | Description |
| --- | --- |
| [isGroupedBy(PivotGroupByType)](#isGroupedBy-pivotgroupbytype-)| Check whether the field is grouped by the type. |
| [getType()](#getType--)| Gets the data time group type. |
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
Readonly. Gets the start date time of the group.
```javascript
start : Date;
```
### end {#end--}
Readonly. Gets the end date time of the group.
```javascript
end : Date;
```
### interval {#interval--}
Readonly. Gets the internal of the group.
```javascript
interval : number;
```
### groupByTypes {#groupByTypes--}
Readonly. Gets the types of grouping by date time.
```javascript
groupByTypes : PivotGroupByType[];
```
### isGroupedBy(PivotGroupByType) {#isGroupedBy-pivotgroupbytype-}
Check whether the field is grouped by the type.
```javascript
isGroupedBy(type: PivotGroupByType) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotGroupByType](../pivotgroupbytype/) | The group type |
### getType() {#getType--}
Gets the data time group type.
```javascript
getType() : PivotFieldGroupType;
```
**Returns**
[PivotFieldGroupType](../pivotfieldgrouptype/)
