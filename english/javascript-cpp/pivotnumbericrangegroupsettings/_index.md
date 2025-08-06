---
title: PivotNumbericRangeGroupSettings
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the numberic range group of the pivot field.
type: docs
url: /javascript-cpp/pivotnumbericrangegroupsettings/
---

## PivotNumbericRangeGroupSettings class

Represents the numberic range group of the pivot field.

```javascript
class PivotNumbericRangeGroupSettings extends PivotFieldGroupSettings;
```


## Constructors

| Name | Description |
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


### getType() {#getType--}

Gets the group type.

```javascript
getType() : PivotFieldGroupType;
```


**Returns**

[PivotFieldGroupType](../pivotfieldgrouptype/)


