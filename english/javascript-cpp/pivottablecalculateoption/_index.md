---
title: PivotTableCalculateOption
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Rerepsents the options of calculating data of the pivot table.
type: docs
url: /javascript-cpp/pivottablecalculateoption/
---

## PivotTableCalculateOption class

Rerepsents the options of calculating data of the pivot table.

```javascript
class PivotTableCalculateOption;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [refreshData](#refreshData--)| boolean | Indicates whether refreshing data source of the pivottable. |
| [refreshCharts](#refreshCharts--)| boolean | Indicates whether refreshing charts are based on this pivot table. |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |
| [refreshOption](#refreshOption--)| PivotTableRefreshOption | Gets and set options for refreshing data source to pivot cache. |


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

Only works when [PivotTableCalculateOption.RefreshData](../pivottablecalculateoption.refreshdata/) is true.

### refreshOption {#refreshOption--}

Gets and set options for refreshing data source to pivot cache.

```javascript
refreshOption : PivotTableRefreshOption;
```



