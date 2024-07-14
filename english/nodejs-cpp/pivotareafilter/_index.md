---
title: PivotAreaFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the filter of PivotAreanodejscpppivotarea for PivotAreanodejscpppivotarea.
type: docs
url: /nodejs-cpp/pivotareafilter/
---

## PivotAreaFilter class

Represents the filter of [PivotArea](/nodejs-cpp/pivotarea/) for [PivotArea](/nodejs-cpp/pivotarea/).

```javascript
class PivotAreaFilter;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getSelected()](#getSelected--)| Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
| [setSelected(boolean)](#setSelected-boolean-)| Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
| [isSubtotalSet(PivotFieldSubtotalType)](#isSubtotalSet-pivotfieldsubtotaltype-)| Gets which subtotal is set for this filter. |
| [setSubtotals(PivotFieldSubtotalType, boolean)](#setSubtotals-pivotfieldsubtotaltype-boolean-)| Subtotal for the filter. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getSelected() {#getSelected--}

Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

```javascript
getSelected() : boolean;
```


### setSelected(boolean) {#setSelected-boolean-}

Indicates whether this field has selection. Only works when the PivotTable is in Outline view.

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
| subtotalType | [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) | The subtotal function type. |

### setSubtotals(PivotFieldSubtotalType, boolean) {#setSubtotals-pivotfieldsubtotaltype-boolean-}

Subtotal for the filter.

```javascript
setSubtotals(subtotalType: PivotFieldSubtotalType, shown: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) | The subtotal function. |
| shown | boolean | Indicates if showing this subtotal data. |


