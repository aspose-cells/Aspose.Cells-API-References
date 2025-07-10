﻿---
title: LoadFilter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the filter that provides options for loading data when loading workbook from template.
type: docs
url: /nodejs-cpp/loadfilter/
---

## LoadFilter class

Represents the filter that provides options for loading data when loading workbook from template.

```javascript
class LoadFilter;
```

### Remarks
User may specify the filter options or implement their own LoadFilter to specify how to load data.

## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
| [constructor(LoadDataFilterOptions)](#constructor-loaddatafilteroptions-)| Constructs one LoadFilter with given filter options. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [loadDataFilterOptions](#loadDataFilterOptions--)| LoadDataFilterOptions | The filter options to denote what data should be loaded. |

## Methods

| Method | Description |
| --- | --- |
| [getLoadDataFilterOptions()](#getLoadDataFilterOptions--)| <b>@deprecated.</b> Please use the 'loadDataFilterOptions' property instead. The filter options to denote what data should be loaded. |
| [setLoadDataFilterOptions(LoadDataFilterOptions)](#setLoadDataFilterOptions-loaddatafilteroptions-)| <b>@deprecated.</b> Please use the 'loadDataFilterOptions' property instead. The filter options to denote what data should be loaded. |
| abstract [getSheetsInLoadingOrder()](#getSheetsInLoadingOrder--)| Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded. |
| abstract [startSheet(Worksheet)](#startSheet-worksheet-)| Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### constructor(LoadDataFilterOptions) {#constructor-loaddatafilteroptions-}

Constructs one LoadFilter with given filter options.

```javascript
constructor(opts: LoadDataFilterOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| opts | [LoadDataFilterOptions](../loaddatafilteroptions/) | The default filter options. |

### loadDataFilterOptions {#loadDataFilterOptions--}

The filter options to denote what data should be loaded.

```javascript
loadDataFilterOptions : LoadDataFilterOptions;
```


### getLoadDataFilterOptions() {#getLoadDataFilterOptions--}

<b>@deprecated.</b> Please use the 'loadDataFilterOptions' property instead. The filter options to denote what data should be loaded.

```javascript
getLoadDataFilterOptions() : LoadDataFilterOptions;
```


**Returns**

[LoadDataFilterOptions](../loaddatafilteroptions/)

### setLoadDataFilterOptions(LoadDataFilterOptions) {#setLoadDataFilterOptions-loaddatafilteroptions-}

<b>@deprecated.</b> Please use the 'loadDataFilterOptions' property instead. The filter options to denote what data should be loaded.

```javascript
setLoadDataFilterOptions(value: LoadDataFilterOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LoadDataFilterOptions](../loaddatafilteroptions/) | The value to set. |

### getSheetsInLoadingOrder() {#getSheetsInLoadingOrder--}

Specifies the sheets(indices) and order to be loaded. Default is null, that denotes to load all sheets in the default order in template file. If not null and some sheet's index is not in the returned array, then the sheet will not be loaded.

```javascript
abstract getSheetsInLoadingOrder() : number[];
```


**Returns**

number[]

### startSheet(Worksheet) {#startSheet-worksheet-}

Prepares filter options before loading given worksheet. User's implementation of LoadFilter can change the LoadDataFilterOptions here to denote how to load data for this worksheet.

```javascript
abstract startSheet(sheet: Worksheet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | [Worksheet](../worksheet/) | The worksheet to be loaded.         /// There are only few properties can be used for the given worksheet object here         /// because most data and properties have not been loaded. The available properties are:         /// Name, Index, VisibilityType |


