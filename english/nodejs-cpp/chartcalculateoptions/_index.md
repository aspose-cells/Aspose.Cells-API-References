---
title: ChartCalculateOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for calculating chart.
type: docs
url: /nodejs-cpp/chartcalculateoptions/
---

## ChartCalculateOptions class

Represents the options for calculating chart.

```javascript
class ChartCalculateOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for calculating chart. |

## Methods

| Method | Description |
| --- | --- |
| [getUpdateAllPoints()](#getUpdateAllPoints--)| Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |
| [setUpdateAllPoints(boolean)](#setUpdateAllPoints-boolean-)| Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger. |


### constructor() {#constructor--}

Creates the options for calculating chart.

```javascript
constructor();
```


### getUpdateAllPoints() {#getUpdateAllPoints--}

Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.

```javascript
getUpdateAllPoints() : boolean;
```


### setUpdateAllPoints(boolean) {#setUpdateAllPoints-boolean-}

Whether update all data points when performing the chart calculation. Default: False. When you want to get the value for each data point in the chart specifically, set it to true. If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.

```javascript
setUpdateAllPoints(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |


