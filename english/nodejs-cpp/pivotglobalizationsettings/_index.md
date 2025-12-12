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
class PivotGlobalizationSettings;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| abstract [getTextOfTotal()](#getTextOfTotal--)| Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area. |
| abstract [getTextOfGrandTotal()](#getTextOfGrandTotal--)| Gets the text of "Grand Total" label in the PivotTable. |
| abstract [getTextOfMultipleItems()](#getTextOfMultipleItems--)| Gets the text of "(Multiple Items)" label in the PivotTable. |
| abstract [getTextOfAll()](#getTextOfAll--)| Gets the text of "(All)" label in the PivotTable. |
| abstract [getTextOfProtectedName(string)](#getTextOfProtectedName-string-)| Gets the text for specified protected name. |
| abstract [getTextOfColumnLabels()](#getTextOfColumnLabels--)| Gets the text of "Column Labels" label in the PivotTable. |
| abstract [getTextOfRowLabels()](#getTextOfRowLabels--)| Gets the text of "Row Labels" label in the PivotTable. |
| abstract [getTextOfEmptyData()](#getTextOfEmptyData--)| Gets the text of "(blank)" label in the PivotTable. |
| abstract [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--)| Gets the the text of the value area field header in the PivotTable. |
| abstract [getShortTextOf12Months()](#getShortTextOf12Months--)| Gets all short formatted string of 12 months. |
| abstract [getTextOf4Quaters()](#getTextOf4Quaters--)| Gets the local text of 4 Quaters. |
| abstract [getTextOfYears()](#getTextOfYears--)| Gets the local text of "Years". |
| abstract [getTextOfQuarters()](#getTextOfQuarters--)| Get the local text of "Quarters". |
| abstract [getTextOfMonths()](#getTextOfMonths--)| Gets the local text of "Months". |
| abstract [getTextOfDays()](#getTextOfDays--)| Gets the local text of "Days". |
| abstract [getTextOfHours()](#getTextOfHours--)| Gets the local text of "Hours". |
| abstract [getTextOfMinutes()](#getTextOfMinutes--)| Gets the local text of "Minutes". |
| abstract [getTextOfSeconds()](#getTextOfSeconds--)| Gets the local text of "Seconds" |
| abstract [getTextOfRange()](#getTextOfRange--)| Gets the local text of "Range" |
| abstract [getTextOfAllPeriods()](#getTextOfAllPeriods--)| Gets the localized text of "All Periods". |
| abstract [getNameOfDataField(ConsolidationFunction, string)](#getNameOfDataField-consolidationfunction-string-)| Gets the display name of data pivot field. The default format is "Sum Of Field". |
| abstract [getTextOfSubTotal(PivotFieldSubtotalType)](#getTextOfSubTotal-pivotfieldsubtotaltype-)| Gets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getTextOfTotal() {#getTextOfTotal--}

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

```javascript
abstract getTextOfTotal() : string;
```


**Returns**

The text of "Total" label

### getTextOfGrandTotal() {#getTextOfGrandTotal--}

Gets the text of "Grand Total" label in the PivotTable.

```javascript
abstract getTextOfGrandTotal() : string;
```


**Returns**

The text of "Grand Total" label

### getTextOfMultipleItems() {#getTextOfMultipleItems--}

Gets the text of "(Multiple Items)" label in the PivotTable.

```javascript
abstract getTextOfMultipleItems() : string;
```


**Returns**

The text of "(Multiple Items)" label

### getTextOfAll() {#getTextOfAll--}

Gets the text of "(All)" label in the PivotTable.

```javascript
abstract getTextOfAll() : string;
```


**Returns**

The text of "(All)" label

### getTextOfProtectedName(string) {#getTextOfProtectedName-string-}

Gets the text for specified protected name.

```javascript
abstract getTextOfProtectedName(protectedName: string) : string;
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
abstract getTextOfColumnLabels() : string;
```


**Returns**

The text of column labels

### getTextOfRowLabels() {#getTextOfRowLabels--}

Gets the text of "Row Labels" label in the PivotTable.

```javascript
abstract getTextOfRowLabels() : string;
```


**Returns**

The text of row labels

### getTextOfEmptyData() {#getTextOfEmptyData--}

Gets the text of "(blank)" label in the PivotTable.

```javascript
abstract getTextOfEmptyData() : string;
```


**Returns**

The text of empty data

### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}

Gets the the text of the value area field header in the PivotTable.

```javascript
abstract getTextOfDataFieldHeader() : string;
```


**Returns**

The text of data field header name

### getShortTextOf12Months() {#getShortTextOf12Months--}

Gets all short formatted string of 12 months.

```javascript
abstract getShortTextOf12Months() : string[];
```


**Returns**

string[]

### getTextOf4Quaters() {#getTextOf4Quaters--}

Gets the local text of 4 Quaters.

```javascript
abstract getTextOf4Quaters() : string[];
```


**Returns**

string[]

### getTextOfYears() {#getTextOfYears--}

Gets the local text of "Years".

```javascript
abstract getTextOfYears() : string;
```


### getTextOfQuarters() {#getTextOfQuarters--}

Get the local text of "Quarters".

```javascript
abstract getTextOfQuarters() : string;
```


### getTextOfMonths() {#getTextOfMonths--}

Gets the local text of "Months".

```javascript
abstract getTextOfMonths() : string;
```


### getTextOfDays() {#getTextOfDays--}

Gets the local text of "Days".

```javascript
abstract getTextOfDays() : string;
```


### getTextOfHours() {#getTextOfHours--}

Gets the local text of "Hours".

```javascript
abstract getTextOfHours() : string;
```


### getTextOfMinutes() {#getTextOfMinutes--}

Gets the local text of "Minutes".

```javascript
abstract getTextOfMinutes() : string;
```


### getTextOfSeconds() {#getTextOfSeconds--}

Gets the local text of "Seconds"

```javascript
abstract getTextOfSeconds() : string;
```


### getTextOfRange() {#getTextOfRange--}

Gets the local text of "Range"

```javascript
abstract getTextOfRange() : string;
```


### getTextOfAllPeriods() {#getTextOfAllPeriods--}

Gets the localized text of "All Periods".

```javascript
abstract getTextOfAllPeriods() : string;
```


### getNameOfDataField(ConsolidationFunction, string) {#getNameOfDataField-consolidationfunction-string-}

Gets the display name of data pivot field. The default format is "Sum Of Field".

```javascript
abstract getNameOfDataField(consolidationFunction: ConsolidationFunction, name: string) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| consolidationFunction | [ConsolidationFunction](../consolidationfunction/) | The function is used to summarize values of pivot field. |
| name | string | The original name of the pivot field. |

### getTextOfSubTotal(PivotFieldSubtotalType) {#getTextOfSubTotal-pivotfieldsubtotaltype-}

Gets the text of [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) type in the PivotTable.

```javascript
abstract getTextOfSubTotal(subTotalType: PivotFieldSubtotalType) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) |

**Returns**

The text of given type


