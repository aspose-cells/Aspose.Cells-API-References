---
title: PivotAreaFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the filter of PivotArea..pivotarea for PivotTable..pivottable.
type: docs
url: /nodejs-cpp/pivotareafilter/
---

## PivotAreaFilter class

Represents the filter of [PivotArea](../pivotarea/) for [PivotTable](../pivottable/).

```javascript
class PivotAreaFilter;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [fieldIndex](#fieldIndex--)| number | Readonly. Gets the index of the field which this filter refers to. A value of -2 indicates the values field. |
| [selected](#selected--)| boolean | Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |

## Methods

| Method | Description |
| --- | --- |
| [getFieldIndex()](#getFieldIndex--)| <b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets the index of the field which this filter refers to. A value of -2 indicates the values field. |
| [getSelected()](#getSelected--)| <b>@deprecated.</b> Please use the 'selected' property instead. Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
| [setSelected(boolean)](#setSelected-boolean-)| <b>@deprecated.</b> Please use the 'selected' property instead. Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
| [isSubtotalSet(PivotFieldSubtotalType)](#isSubtotalSet-pivotfieldsubtotaltype-)| Gets which subtotal is set for this filter. |
| [setSubtotals(PivotFieldSubtotalType, boolean)](#setSubtotals-pivotfieldsubtotaltype-boolean-)| Subtotal for the filter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### fieldIndex {#fieldIndex--}

Readonly. Gets the index of the field which this filter refers to. A value of -2 indicates the values field.

```javascript
fieldIndex : number;
```


### selected {#selected--}

Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

```javascript
selected : boolean;
```


### getFieldIndex() {#getFieldIndex--}

<b>@deprecated.</b> Please use the 'fieldIndex' property instead. Gets the index of the field which this filter refers to. A value of -2 indicates the values field.

```javascript
getFieldIndex() : number;
```


### getSelected() {#getSelected--}

<b>@deprecated.</b> Please use the 'selected' property instead. Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

```javascript
getSelected() : boolean;
```


### setSelected(boolean) {#setSelected-boolean-}

<b>@deprecated.</b> Please use the 'selected' property instead. Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

```javascript
setSelected(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isSubtotalSet(PivotFieldSubtotalType) {#isSubtotalSet-pivotfieldsubtotaltype-}

Gets which subtotal is set for this filter.

```javascript
isSubtotalSet(subtotalType: PivotFieldSubtotalType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal function type. |

### setSubtotals(PivotFieldSubtotalType, boolean) {#setSubtotals-pivotfieldsubtotaltype-boolean-}

Subtotal for the filter.

```javascript
setSubtotals(subtotalType: PivotFieldSubtotalType, shown: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal function. |
| shown | boolean | Indicates if showing this subtotal data. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



