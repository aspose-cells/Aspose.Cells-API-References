---
title: PivotTableCalculateOption
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Rerepsents the options of calculating data of the pivot table.
type: docs
url: /nodejs-cpp/pivottablecalculateoption/
---

## PivotTableCalculateOption class

Rerepsents the options of calculating data of the pivot table.

```javascript
class PivotTableCalculateOption;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [refreshData](#refreshData--)| boolean | Indicates whether refreshing data source of the pivottable. |
| [refreshCharts](#refreshCharts--)| boolean | Indicates whether refreshing charts are based on this pivot table. |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |

## Methods

| Method | Description |
| --- | --- |
| [getRefreshData()](#getRefreshData--)| <b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable. |
| [setRefreshData(boolean)](#setRefreshData-boolean-)| <b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable. |
| [getRefreshCharts()](#getRefreshCharts--)| <b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table. |
| [setRefreshCharts(boolean)](#setRefreshCharts-boolean-)| <b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [setReserveMissingPivotItemType(ReserveMissingPivotItemType)](#setReserveMissingPivotItemType-reservemissingpivotitemtype-)| <b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### refreshData {#refreshData--}

Indicates whether refreshing data source of the pivottable.

```javascript
refreshData : boolean;
```


**Remarks**

If it is true, refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### refreshCharts {#refreshCharts--}

Indicates whether refreshing charts are based on this pivot table.

```javascript
refreshCharts : boolean;
```


### reserveMissingPivotItemType {#reserveMissingPivotItemType--}

Represents how to reserve missing pivot items.

```javascript
reserveMissingPivotItemType : ReserveMissingPivotItemType;
```


**Remarks**

Only works when [RefreshData](../refreshdata/) is true.

### getRefreshData() {#getRefreshData--}

<b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable.

```javascript
getRefreshData() : boolean;
```


**Remarks**

If it is true, refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### setRefreshData(boolean) {#setRefreshData-boolean-}

<b>@deprecated.</b> Please use the 'refreshData' property instead. Indicates whether refreshing data source of the pivottable.

```javascript
setRefreshData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If it is true, refresh pivot cache from data source,then calculate all pivot tables based same pivot cache.

### getRefreshCharts() {#getRefreshCharts--}

<b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table.

```javascript
getRefreshCharts() : boolean;
```


### setRefreshCharts(boolean) {#setRefreshCharts-boolean-}

<b>@deprecated.</b> Please use the 'refreshCharts' property instead. Indicates whether refreshing charts are based on this pivot table.

```javascript
setRefreshCharts(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}

<b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items.

```javascript
getReserveMissingPivotItemType() : ReserveMissingPivotItemType;
```


**Returns**

[ReserveMissingPivotItemType](../reservemissingpivotitemtype/)

**Remarks**

Only works when [RefreshData](../refreshdata/) is true.

### setReserveMissingPivotItemType(ReserveMissingPivotItemType) {#setReserveMissingPivotItemType-reservemissingpivotitemtype-}

<b>@deprecated.</b> Please use the 'reserveMissingPivotItemType' property instead. Represents how to reserve missing pivot items.

```javascript
setReserveMissingPivotItemType(value: ReserveMissingPivotItemType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ReserveMissingPivotItemType](../reservemissingpivotitemtype/) | The value to set. |

**Remarks**

Only works when [RefreshData](../refreshdata/) is true.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



