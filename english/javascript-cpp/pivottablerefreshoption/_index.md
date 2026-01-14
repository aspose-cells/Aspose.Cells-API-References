---
title: PivotTableRefreshOption
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the options of refreshing data source of the pivot table.
type: docs
url: /javascript-cpp/pivottablerefreshoption/
---

## PivotTableRefreshOption class

Represents the options of refreshing data source of the pivot table.

```javascript
class PivotTableRefreshOption;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Represents the options of refreshing data source of the pivot table. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [reserveMissingPivotItemType](#reserveMissingPivotItemType--)| ReserveMissingPivotItemType | Represents how to reserve missing pivot items. |
| [isKeepOriginalOrder](#isKeepOriginalOrder--)| boolean | Indicates whether to keep pivot items' original order as old data source. |


### constructor() {#constructor--}

Represents the options of refreshing data source of the pivot table.

```javascript
constructor();
```


### reserveMissingPivotItemType {#reserveMissingPivotItemType--}

Represents how to reserve missing pivot items.

```javascript
reserveMissingPivotItemType : ReserveMissingPivotItemType;
```


### isKeepOriginalOrder {#isKeepOriginalOrder--}

Indicates whether to keep pivot items' original order as old data source.

```javascript
isKeepOriginalOrder : boolean;
```


**Remarks**

Only applicable for the pivot field which is not sorted. When refreshing such kind of pivot field, Ms Excel keeps the original order of old data source. Default value of this property is true, representing the same behavior with Ms Excel. If user needs the pivot field to be refreshed completely as the data in the new data source, this property should be set as false.


