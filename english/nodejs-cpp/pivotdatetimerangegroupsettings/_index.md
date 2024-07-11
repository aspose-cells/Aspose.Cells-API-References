---
title: PivotDateTimeRangeGroupSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the field grouped by date time range.
type: docs
url: /nodejs-cpp/pivotdatetimerangegroupsettings/
---

## PivotDateTimeRangeGroupSettings class

Represents the field grouped by date time range.

```javascript
class PivotDateTimeRangeGroupSettings extends PivotFieldGroupSettings;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PivotFieldGroupSettings)](#constructor-pivotfieldgroupsettings-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the data time group type. |
| [getStart()](#getStart--)| Gets the start date time of the group. |
| [getEnd()](#getEnd--)| Gets the end date time of the group. |
| [getInterval()](#getInterval--)| Gets the internal of the group. |
| [getGroupByTypes()](#getGroupByTypes--)| Gets the types of grouping by date time. |
| [isGroupedBy(PivotGroupByType)](#isGroupedBy-pivotgroupbytype-)| Check whether the field is grouped by the type. |


### constructor(PivotFieldGroupSettings) {#constructor-pivotfieldgroupsettings-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: PivotFieldGroupSettings);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PivotFieldGroupSettings | The parent object. |

### getType() {#getType--}

Gets the data time group type.

```javascript
getType() : PivotFieldGroupType;
```


**Returns**

[PivotFieldGroupType](./pivotfieldgrouptype/)

### getStart() {#getStart--}

Gets the start date time of the group.

```javascript
getStart() : Date;
```


### getEnd() {#getEnd--}

Gets the end date time of the group.

```javascript
getEnd() : Date;
```


### getInterval() {#getInterval--}

Gets the internal of the group.

```javascript
getInterval() : number;
```


### getGroupByTypes() {#getGroupByTypes--}

Gets the types of grouping by date time.

```javascript
getGroupByTypes() : PivotGroupByType[];
```


**Returns**

[PivotGroupByType](./pivotgroupbytype/)[]

### isGroupedBy(PivotGroupByType) {#isGroupedBy-pivotgroupbytype-}

Check whether the field is grouped by the type.

```javascript
isGroupedBy(type: PivotGroupByType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [PivotGroupByType](./pivotgroupbytype/) | The group type |


