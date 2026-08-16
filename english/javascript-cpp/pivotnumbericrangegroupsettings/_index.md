---
title: PivotNumbericRangeGroupSettings
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the numeric range group of the pivot field.
type: docs
url: /javascript-cpp/pivotnumbericrangegroupsettings/
---

## PivotNumbericRangeGroupSettings class

Represents the numeric range group of the pivot field.

```javascript
class PivotNumbericRangeGroupSettings extends PivotNumericRangeGroupSettings;
```

### Remarks
NOTE: This class is now obsolete. Instead, please use PivotNumericRangeGroupSettings class instead . This method will be removed 6 months later since July 2026. Aspose apologizes for any inconvenience you may have experienced.

## Constructors

| Name | Description |
| --- | --- |
| [constructor(PivotNumericRangeGroupSettings)](#constructor-pivotnumericrangegroupsettings-)| Constructs from a parent object convertible to this. |

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


### constructor(PivotNumericRangeGroupSettings) {#constructor-pivotnumericrangegroupsettings-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: PivotNumericRangeGroupSettings);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PivotNumericRangeGroupSettings | The parent object. |

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


