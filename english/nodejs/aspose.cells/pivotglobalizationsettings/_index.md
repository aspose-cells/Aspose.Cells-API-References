---
title: "PivotGlobalizationSettings"
linktitle: "PivotGlobalizationSettings"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the globalization settings for pivot tables."
type: docs
weight: 2830
url: /nodejs/aspose.cells/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Represents the globalization settings for pivot tables.

```js
new PivotGlobalizationSettings()
```

## Methods

| Name | Description |
| --- | --- |
| [getNameOfDataField()](#getnameofdatafield) |  |
| [getShortTextOf12Months()](#getshorttextof12months) | Gets all short formatted string of 12 months. |
| [getTextOf4Quaters()](#gettextof4quaters) | Gets the local text of 4 Quaters. |
| [getTextOfAll()](#gettextofall) | Gets the text of "(All)" label in the PivotTable. |
| [getTextOfAllPeriods()](#gettextofallperiods) |  |
| [getTextOfColumnLabels()](#gettextofcolumnlabels) | Gets the text of "Column Labels" label in the PivotTable. |
| [getTextOfDataFieldHeader()](#gettextofdatafieldheader) | Gets the the text of the value area field header in the PivotTable. |
| [getTextOfDays()](#gettextofdays) | Gets the local text of "Days". |
| [getTextOfEmptyData()](#gettextofemptydata) | Gets the text of "(blank)" label in the PivotTable. |
| [getTextOfGrandTotal()](#gettextofgrandtotal) | Gets the text of "Grand Total" label in the PivotTable. |
| [getTextOfHours()](#gettextofhours) | Gets the local text of "Hours". |
| [getTextOfMinutes()](#gettextofminutes) | Gets the local text of "Minutes". |
| [getTextOfMonths()](#gettextofmonths) | Gets the local text of "Months". |
| [getTextOfMultipleItems()](#gettextofmultipleitems) | Gets the text of "(Multiple Items)" label in the PivotTable. |
| [getTextOfProtectedName(protectedName)](#gettextofprotectedname) | Gets the text for specified protected name. In Ms Excel, some names are not allowed to be used as the name of PivotField |
| [getTextOfProtection()](#gettextofprotection) | Gets the protection name in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSet |
| [getTextOfQuarters()](#gettextofquarters) | Get the local text of "Quarters". |
| [getTextOfRange()](#gettextofrange) | Gets the local text of "Range" |
| [getTextOfRowLabels()](#gettextofrowlabels) | Gets the text of "Row Labels" label in the PivotTable. |
| [getTextOfSeconds()](#gettextofseconds) | Gets the local text of "Seconds" |
| [getTextOfSubTotal(subTotalType)](#gettextofsubtotal) | Gets the text of PivotFieldSubtotalType type in the PivotTable. |
| [getTextOfTotal()](#gettextoftotal) | Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or m |
| [getTextOfYears()](#gettextofyears) | Gets the local text of "Years". |

### getNameOfDataField() {#getnameofdatafield}

### getShortTextOf12Months() {#getshorttextof12months}

Gets all short formatted string of 12 months.

**Returns:** Array of String — `Array of String`

### getTextOf4Quaters() {#gettextof4quaters}

Gets the local text of 4 Quaters.

**Returns:** Array of String — `Array of String`

### getTextOfAll() {#gettextofall}

Gets the text of "(All)" label in the PivotTable.

**Returns:** String — `String` The text of "(All)" label

### getTextOfAllPeriods() {#gettextofallperiods}

### getTextOfColumnLabels() {#gettextofcolumnlabels}

Gets the text of "Column Labels" label in the PivotTable.

**Returns:** String — `String` The text of column labels

### getTextOfDataFieldHeader() {#gettextofdatafieldheader}

Gets the the text of the value area field header in the PivotTable.

**Returns:** String — `String` The text of data field header name

### getTextOfDays() {#gettextofdays}

Gets the local text of "Days".

**Returns:** String — `String`

### getTextOfEmptyData() {#gettextofemptydata}

Gets the text of "(blank)" label in the PivotTable.

**Returns:** String — `String` The text of empty data

### getTextOfGrandTotal() {#gettextofgrandtotal}

Gets the text of "Grand Total" label in the PivotTable.

**Returns:** String — `String` The text of "Grand Total" label

### getTextOfHours() {#gettextofhours}

Gets the local text of "Hours".

**Returns:** String — `String`

### getTextOfMinutes() {#gettextofminutes}

Gets the local text of "Minutes".

**Returns:** String — `String`

### getTextOfMonths() {#gettextofmonths}

Gets the local text of "Months".

**Returns:** String — `String`

### getTextOfMultipleItems() {#gettextofmultipleitems}

Gets the text of "(Multiple Items)" label in the PivotTable.

**Returns:** String — `String` The text of "(Multiple Items)" label

### getTextOfProtectedName(protectedName) {#gettextofprotectedname}

Gets the text for specified protected name. In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |

**Returns:** String — `String` The local prorected names of PivotTable.

### getTextOfProtection() {#gettextofprotection}

Gets the protection name in the PivotTable. NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.@return {String} The protection name of PivotTable

### getTextOfQuarters() {#gettextofquarters}

Get the local text of "Quarters".

**Returns:** String — `String`

### getTextOfRange() {#gettextofrange}

Gets the local text of "Range"

**Returns:** String — `String`

### getTextOfRowLabels() {#gettextofrowlabels}

Gets the text of "Row Labels" label in the PivotTable.

**Returns:** String — `String` The text of row labels

### getTextOfSeconds() {#gettextofseconds}

Gets the local text of "Seconds"

**Returns:** String — `String`

### getTextOfSubTotal(subTotalType) {#gettextofsubtotal}

Gets the text of PivotFieldSubtotalType type in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | Number | PivotFieldSubtotalType |

**Returns:** String — `String` The text of given type

### getTextOfTotal() {#gettextoftotal}

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

**Returns:** String — `String` The text of "Total" label

### getTextOfYears() {#gettextofyears}

Gets the local text of "Years".

**Returns:** String — `String`
