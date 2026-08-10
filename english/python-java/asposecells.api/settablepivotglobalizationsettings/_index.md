---
title: "SettablePivotGlobalizationSettings Class"
linktitle: "SettablePivotGlobalizationSettings"
articleTitle: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells for Python via Java"
description: "Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts."
type: docs
weight: 5780
url: /python-java/asposecells.api/settablepivotglobalizationsettings/
---

## SettablePivotGlobalizationSettings class

Implementation of PivotGlobalizationSettings that supports user to set/change pre-defined texts.

## Constructors

| Name | Description |
| --- | --- |
| [SettablePivotGlobalizationSettings](#constructor) |  |

## Methods

| Name | Description |
| --- | --- |
| [getTextOfTotal](#gettextoftotal) | Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or m |
| [setTextOfTotal](#settextoftotal) | Sets the text of "Total" label in the PivotTable. |
| [getTextOfGrandTotal](#gettextofgrandtotal) | Gets the text of "Grand Total" label in the PivotTable. |
| [setTextOfGrandTotal](#settextofgrandtotal) | Sets the text of "Grand Total" label in the PivotTable. |
| [getTextOfMultipleItems](#gettextofmultipleitems) | Gets the text of "(Multiple Items)" label in the PivotTable. |
| [setTextOfMultipleItems](#settextofmultipleitems) | Sets the text of "(Multiple Items)" label in the PivotTable. |
| [getTextOfAll](#gettextofall) | Gets the text of "(All)" label in the PivotTable. |
| [setTextOfAll](#settextofall) | Sets the text of "(All)" label in the PivotTable. |
| [getTextOfProtectedName](#gettextofprotectedname) | Gets the text for specified protected name.

In Ms Excel, some names are not allowed to be used as the name of PivotFiel |
| [setTextOfProtectedName](#settextofprotectedname) | Sets the text for specific protected name. |
| [getTextOfColumnLabels](#gettextofcolumnlabels) | Gets the text of "Column Labels" label in the PivotTable. |
| [setTextOfColumnLabels](#settextofcolumnlabels) | Gets the text of "Column Labels" label in the PivotTable. |
| [getTextOfRowLabels](#gettextofrowlabels) | Gets the text of "Row Labels" label in the PivotTable. |
| [setTextOfRowLabels](#settextofrowlabels) | Sets the text of "Row Labels" label in the PivotTable. |
| [getTextOfEmptyData](#gettextofemptydata) | Gets the text of "(blank)" label in the PivotTable. |
| [setTextOfEmptyData](#settextofemptydata) | Sets the text of "(blank)" label in the PivotTable. |
| [getTextOfDataFieldHeader](#gettextofdatafieldheader) | Gets the the text of the value area field header in the PivotTable. |
| [setTextOfDataFieldHeader](#settextofdatafieldheader) | Sets the the text of the value area field header in the PivotTable. |
| [getTextOfSubTotal](#gettextofsubtotal) | Gets the text of PivotFieldSubtotalType type in the PivotTable. |
| [setTextOfSubTotal](#settextofsubtotal) | Sets the text of PivotFieldSubtotalType type in the PivotTable. |
| [getTextOfProtection](#gettextofprotection) | Gets the protection name in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSe |
| [getShortTextOf12Months](#getshorttextof12months) | Gets all short formatted string of 12 months. |
| [getTextOf4Quaters](#gettextof4quaters) | Gets the local text of 4 Quaters. |
| [getTextOfYears](#gettextofyears) | Gets the local text of "Years". |
| [getTextOfQuarters](#gettextofquarters) | Get the local text of "Quarters". |
| [getTextOfMonths](#gettextofmonths) | Gets the local text of "Months". |
| [getTextOfDays](#gettextofdays) | Gets the local text of "Days". |
| [getTextOfHours](#gettextofhours) | Gets the local text of "Hours". |
| [getTextOfMinutes](#gettextofminutes) | Gets the local text of "Minutes". |
| [getTextOfSeconds](#gettextofseconds) | Gets the local text of "Seconds" |
| [getTextOfRange](#gettextofrange) | Gets the local text of "Range" |
| [getTextOfAllPeriods](#gettextofallperiods) |  |
| [getNameOfDataField](#getnameofdatafield) |  |

### SettablePivotGlobalizationSettings() {#constructor}

### getTextOfTotal() {#gettextoftotal}

Gets the text of "Total" label in the PivotTable. You need to override this method when the PivotTable contains two or more PivotFields in the data area.

**Returns:** The text of "Total" label

### setTextOfTotal(text) {#settextoftotal}

Sets the text of "Total" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### getTextOfGrandTotal() {#gettextofgrandtotal}

Gets the text of "Grand Total" label in the PivotTable.

**Returns:** The text of "Grand Total" label

### setTextOfGrandTotal(text) {#settextofgrandtotal}

Sets the text of "Grand Total" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### getTextOfMultipleItems() {#gettextofmultipleitems}

Gets the text of "(Multiple Items)" label in the PivotTable.

**Returns:** The text of "(Multiple Items)" label

### setTextOfMultipleItems(text) {#settextofmultipleitems}

Sets the text of "(Multiple Items)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### getTextOfAll() {#gettextofall}

Gets the text of "(All)" label in the PivotTable.

**Returns:** The text of "(All)" label

### setTextOfAll(text) {#settextofall}

Sets the text of "(All)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | custom text |

### getTextOfProtectedName(protectedName) {#gettextofprotectedname}

Gets the text for specified protected name.

In Ms Excel, some names are not allowed to be used as the name of PivotFields in PivotTable. They are different in different region, user may specify them explicitly according to the used region.

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |

**Returns:** The local prorected names of PivotTable.

### setTextOfProtectedName(protectedName, text) {#settextofprotectedname}

Sets the text for specific protected name.

| Parameter | Type | Description |
| --- | --- | --- |
| protectedName | String | The protected name in PivotTable. |
| text | String | The local prorected names of PivotTable. |

### getTextOfColumnLabels() {#gettextofcolumnlabels}

Gets the text of "Column Labels" label in the PivotTable.

**Returns:** The text of column labels

### setTextOfColumnLabels(text) {#settextofcolumnlabels}

Gets the text of "Column Labels" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of column labels |

### getTextOfRowLabels() {#gettextofrowlabels}

Gets the text of "Row Labels" label in the PivotTable.

**Returns:** The text of row labels

### setTextOfRowLabels(text) {#settextofrowlabels}

Sets the text of "Row Labels" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of row labels |

### getTextOfEmptyData() {#gettextofemptydata}

Gets the text of "(blank)" label in the PivotTable.

**Returns:** The text of empty data

### setTextOfEmptyData(text) {#settextofemptydata}

Sets the text of "(blank)" label in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of empty data |

### getTextOfDataFieldHeader() {#gettextofdatafieldheader}

Gets the the text of the value area field header in the PivotTable.

**Returns:** The text of data field header name

### setTextOfDataFieldHeader(text) {#settextofdatafieldheader}

Sets the the text of the value area field header in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text of data field header name |

### getTextOfSubTotal(subTotalType) {#gettextofsubtotal}

Gets the text of PivotFieldSubtotalType type in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | A PivotFieldSubtotalType value. The PivotFieldSubtotalType |

**Returns:** The text of given type

### setTextOfSubTotal(subTotalType, text) {#settextofsubtotal}

Sets the text of PivotFieldSubtotalType type in the PivotTable.

| Parameter | Type | Description |
| --- | --- | --- |
| subTotalType | int | A PivotFieldSubtotalType value. The PivotFieldSubtotalType |
| text | String | The text of given type |

### getTextOfProtection() {#gettextofprotection}

Gets the protection name in the PivotTable.

NOTE: This member is now obsolete. Instead, please use PivotGlobalizationSettings.GetTextOfProtectedName(string) method. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** The protection name of PivotTable

### getShortTextOf12Months() {#getshorttextof12months}

Gets all short formatted string of 12 months.

### getTextOf4Quaters() {#gettextof4quaters}

Gets the local text of 4 Quaters.

### getTextOfYears() {#gettextofyears}

Gets the local text of "Years".

### getTextOfQuarters() {#gettextofquarters}

Get the local text of "Quarters".

### getTextOfMonths() {#gettextofmonths}

Gets the local text of "Months".

### getTextOfDays() {#gettextofdays}

Gets the local text of "Days".

### getTextOfHours() {#gettextofhours}

Gets the local text of "Hours".

### getTextOfMinutes() {#gettextofminutes}

Gets the local text of "Minutes".

### getTextOfSeconds() {#gettextofseconds}

Gets the local text of "Seconds"

### getTextOfRange() {#gettextofrange}

Gets the local text of "Range"

### getTextOfAllPeriods() {#gettextofallperiods}

### getNameOfDataField(function, name) {#getnameofdatafield}
