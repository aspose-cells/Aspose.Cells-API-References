---
title: PivotGlobalizationSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the globalization settings for pivot tables.
type: docs
url: /nodejs-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Represents the globalization settings for pivot tables.

```javascript
abstract class PivotGlobalizationSettings;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getTextOfTotal()](#getTextOfTotal--)| Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--)| Gets the text of "Grand Total" label in the PivotTable. |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--)| Gets the text of "(Multiple Items)" label in the PivotTable. |
| [getTextOfAll()](#getTextOfAll--)| Gets the text of "(All)" label in the PivotTable. |
| [getTextOfProtectedName(string)](#getTextOfProtectedName-string-)| Gets the text for specified protected name. |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--)| Gets the text of "Column Labels" label in the PivotTable. |
| [getTextOfRowLabels()](#getTextOfRowLabels--)| Gets the text of "Row Labels" label in the PivotTable. |
| [getTextOfEmptyData()](#getTextOfEmptyData--)| Gets the text of "(blank)" label in the PivotTable. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--)| Gets the the text of the value area field header in the PivotTable. |
| [getShortTextOf12Months()](#getShortTextOf12Months--)| Gets all short formatted string of 12 months. |
| [getTextOf4Quaters()](#getTextOf4Quaters--)| Gets the local text of 4 Quaters. |
| [getTextOfYears()](#getTextOfYears--)| Gets the local text of "Years". |
| [getTextOfQuarters()](#getTextOfQuarters--)| Get the local text of "Quarters". |
| [getTextOfMonths()](#getTextOfMonths--)| Gets the local text of "Months". |
| [getTextOfDays()](#getTextOfDays--)| Gets the local text of "Days". |
| [getTextOfHours()](#getTextOfHours--)| Gets the local text of "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--)| Gets the local text of "Minutes". |
| [getTextOfSeconds()](#getTextOfSeconds--)| Gets the local text of "Seconds" |
| [getTextOfRange()](#getTextOfRange--)| Gets the local text of "Range" |
| [getTextOfSubTotal(PivotFieldSubtotalType)](#getTextOfSubTotal-pivotfieldsubtotaltype-)| Gets the text of [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) type in the PivotTable. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getTextOfTotal() {#getTextOfTotal--}

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

```javascript
getTextOfTotal() : string;
```


**Returns**

The text of "Total" label

### getTextOfGrandTotal() {#getTextOfGrandTotal--}

Gets the text of "Grand Total" label in the PivotTable.

```javascript
getTextOfGrandTotal() : string;
```


**Returns**

The text of "Grand Total" label

### getTextOfMultipleItems() {#getTextOfMultipleItems--}

Gets the text of "(Multiple Items)" label in the PivotTable.

```javascript
getTextOfMultipleItems() : string;
```


**Returns**

The text of "(Multiple Items)" label

### getTextOfAll() {#getTextOfAll--}

Gets the text of "(All)" label in the PivotTable.

```javascript
getTextOfAll() : string;
```


**Returns**

The text of "(All)" label

### getTextOfProtectedName(string) {#getTextOfProtectedName-string-}

Gets the text for specified protected name.

```javascript
getTextOfProtectedName(protectedName: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | string | The protected name in PivotTable. |

**Returns**

The local prorected names of PivotTable.

**Remarks**

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

### getTextOfColumnLabels() {#getTextOfColumnLabels--}

Gets the text of "Column Labels" label in the PivotTable.

```javascript
getTextOfColumnLabels() : string;
```


**Returns**

The text of column labels

### getTextOfRowLabels() {#getTextOfRowLabels--}

Gets the text of "Row Labels" label in the PivotTable.

```javascript
getTextOfRowLabels() : string;
```


**Returns**

The text of row labels

### getTextOfEmptyData() {#getTextOfEmptyData--}

Gets the text of "(blank)" label in the PivotTable.

```javascript
getTextOfEmptyData() : string;
```


**Returns**

The text of empty data

### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}

Gets the the text of the value area field header in the PivotTable.

```javascript
getTextOfDataFieldHeader() : string;
```


**Returns**

The text of data field header name

### getShortTextOf12Months() {#getShortTextOf12Months--}

Gets all short formatted string of 12 months.

```javascript
getShortTextOf12Months() : string[];
```


**Returns**

string[]

### getTextOf4Quaters() {#getTextOf4Quaters--}

Gets the local text of 4 Quaters.

```javascript
getTextOf4Quaters() : string[];
```


**Returns**

string[]

### getTextOfYears() {#getTextOfYears--}

Gets the local text of "Years".

```javascript
getTextOfYears() : string;
```


### getTextOfQuarters() {#getTextOfQuarters--}

Get the local text of "Quarters".

```javascript
getTextOfQuarters() : string;
```


### getTextOfMonths() {#getTextOfMonths--}

Gets the local text of "Months".

```javascript
getTextOfMonths() : string;
```


### getTextOfDays() {#getTextOfDays--}

Gets the local text of "Days".

```javascript
getTextOfDays() : string;
```


### getTextOfHours() {#getTextOfHours--}

Gets the local text of "Hours".

```javascript
getTextOfHours() : string;
```


### getTextOfMinutes() {#getTextOfMinutes--}

Gets the local text of "Minutes".

```javascript
getTextOfMinutes() : string;
```


### getTextOfSeconds() {#getTextOfSeconds--}

Gets the local text of "Seconds"

```javascript
getTextOfSeconds() : string;
```


### getTextOfRange() {#getTextOfRange--}

Gets the local text of "Range"

```javascript
getTextOfRange() : string;
```


### getTextOfSubTotal(PivotFieldSubtotalType) {#getTextOfSubTotal-pivotfieldsubtotaltype-}

Gets the text of [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) type in the PivotTable.

```javascript
getTextOfSubTotal(subTotalType: PivotFieldSubtotalType) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) | The [PivotFieldSubtotalType](/nodejs-cpp/pivotfieldsubtotaltype/) |

**Returns**

The text of given type


