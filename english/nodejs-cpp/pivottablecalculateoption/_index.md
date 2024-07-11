---
title: PivotTableCalculateOption
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Rerepsents the options of calcuating the pivot table.
type: docs
url: /nodejs-cpp/pivottablecalculateoption/
---

## PivotTableCalculateOption class

Rerepsents the options of calcuating the pivot table.

```javascript
class PivotTableCalculateOption;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getRefreshData()](#getRefreshData--)| Indicates whether refreshing data source of the pivottable. |
| [setRefreshData(boolean)](#setRefreshData-boolean-)| Indicates whether refreshing data source of the pivottable. |
| [getRefreshCharts()](#getRefreshCharts--)| Indicates whether refreshing charts are based on this pivot table. |
| [setRefreshCharts(boolean)](#setRefreshCharts-boolean-)| Indicates whether refreshing charts are based on this pivot table. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--)| Represents how to reserve missing pivot items. |
| [setReserveMissingPivotItemType(ReserveMissingPivotItemType)](#setReserveMissingPivotItemType-reservemissingpivotitemtype-)| Represents how to reserve missing pivot items. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getRefreshData() {#getRefreshData--}

Indicates whether refreshing data source of the pivottable.

```javascript
getRefreshData() : boolean;
```


### setRefreshData(boolean) {#setRefreshData-boolean-}

Indicates whether refreshing data source of the pivottable.

```javascript
setRefreshData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshCharts() {#getRefreshCharts--}

Indicates whether refreshing charts are based on this pivot table.

```javascript
getRefreshCharts() : boolean;
```


### setRefreshCharts(boolean) {#setRefreshCharts-boolean-}

Indicates whether refreshing charts are based on this pivot table.

```javascript
setRefreshCharts(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}

Represents how to reserve missing pivot items.

```javascript
getReserveMissingPivotItemType() : ReserveMissingPivotItemType;
```


**Returns**

[ReserveMissingPivotItemType](./reservemissingpivotitemtype/)

**Remarks**

Only works when [RefreshData](./refreshdata/) is true.

### setReserveMissingPivotItemType(ReserveMissingPivotItemType) {#setReserveMissingPivotItemType-reservemissingpivotitemtype-}

Represents how to reserve missing pivot items.

```javascript
setReserveMissingPivotItemType(value: ReserveMissingPivotItemType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReserveMissingPivotItemType](./reservemissingpivotitemtype/) | The value to set. |

**Remarks**

Only works when [RefreshData](./refreshdata/) is true.


