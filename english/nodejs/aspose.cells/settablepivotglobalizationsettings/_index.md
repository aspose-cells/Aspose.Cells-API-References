---
title: "SettablePivotGlobalizationSettings"
linktitle: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts."
type: docs
weight: 3530
url: /nodejs/aspose.cells/settablepivotglobalizationsettings/
---

## SettablePivotGlobalizationSettings class

Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.

```js
new SettablePivotGlobalizationSettings()
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
| [setTextOfAll(text)](#settextofall) | Sets the text of "(All)" label in the PivotTable. |
| [setTextOfColumnLabels(text)](#settextofcolumnlabels) | Gets the text of "Column Labels" label in the PivotTable. |
| [setTextOfDataFieldHeader(text)](#settextofdatafieldheader) | Sets the the text of the value area field header in the PivotTable. |
| [setTextOfEmptyData(text)](#settextofemptydata) | Sets the text of "(blank)" label in the PivotTable. |
| [setTextOfGrandTotal(text)](#settextofgrandtotal) | Sets the text of "Grand Total" label in the PivotTable. |
| [setTextOfMultipleItems(text)](#settextofmultipleitems) | Sets the text of "(Multiple Items)" label in the PivotTable. |
| [setTextOfProtectedName(protectedName, text)](#settextofprotectedname) | Sets the text for specific protected name. |
| [setTextOfRowLabels(text)](#settextofrowlabels) | Sets the text of "Row Labels" label in the PivotTable. |
| [setTextOfSubTotal(subTotalType, text)](#settextofsubtotal) | Sets the text of PivotFieldSubtotalType type in the PivotTable. |
| [setTextOfTotal(text)](#settextoftotal) | Sets the text of "Total" label in the PivotTable. |

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

### setTextOfAll(text) {#settextofall}

Sets the text of "(All)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### setTextOfColumnLabels(text) {#settextofcolumnlabels}

Gets the text of "Column Labels" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of column labels |

### setTextOfDataFieldHeader(text) {#settextofdatafieldheader}

Sets the the text of the value area field header in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of data field header name |

### setTextOfEmptyData(text) {#settextofemptydata}

Sets the text of "(blank)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of empty data |

### setTextOfGrandTotal(text) {#settextofgrandtotal}

Sets the text of "Grand Total" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### setTextOfMultipleItems(text) {#settextofmultipleitems}

Sets the text of "(Multiple Items)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### setTextOfProtectedName(protectedName, text) {#settextofprotectedname}

Sets the text for specific protected name.

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |
| text | String | The local prorected names of PivotTable. |

### setTextOfRowLabels(text) {#settextofrowlabels}

Sets the text of "Row Labels" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of row labels |

### setTextOfSubTotal(subTotalType, text) {#settextofsubtotal}

Sets the text of PivotFieldSubtotalType type in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | Number | PivotFieldSubtotalType |
| text | String | The text of given type |

### setTextOfTotal(text) {#settextoftotal}

Sets the text of "Total" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |
