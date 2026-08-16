---
title: PivotDiscreteGroupSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Rrepsents the discrete group of pivot field
type: docs
url: /nodejs-cpp/pivotdiscretegroupsettings/
---

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
| [discreteItems](#discreteItems--)| DiscreteGroupItem[] | Readonly. Gets the discrete items. |

## Methods

| Method | Description |
| --- | --- |
| [getItems()](#getItems--)| <b>@deprecated.</b> Please use the 'items' property instead. Gets the discrete items. |
| [getDiscreteItems()](#getDiscreteItems--)| <b>@deprecated.</b> Please use the 'discreteItems' property instead. Gets the discrete items. |
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


**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy(DiscreteGroupItem[], bool) method . This method will be removed 12 months later since July 2026. Aspose apologizes for any inconvenience you may have experienced.

### discreteItems {#discreteItems--}

Readonly. Gets the discrete items.

```javascript
discreteItems : DiscreteGroupItem[];
```


### getItems() {#getItems--}

<b>@deprecated.</b> Please use the 'items' property instead. Gets the discrete items.

```javascript
getItems() : CustomPiovtFieldGroupItem[];
```


**Returns**

[CustomPiovtFieldGroupItem](../custompiovtfieldgroupitem/)[]

**Remarks**

NOTE: This method is now obsolete. Instead, please use PivotField.GroupBy(DiscreteGroupItem[], bool) method . This method will be removed 12 months later since July 2026. Aspose apologizes for any inconvenience you may have experienced.

### getDiscreteItems() {#getDiscreteItems--}

<b>@deprecated.</b> Please use the 'discreteItems' property instead. Gets the discrete items.

```javascript
getDiscreteItems() : DiscreteGroupItem[];
```


**Returns**

[DiscreteGroupItem](../discretegroupitem/)[]

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


