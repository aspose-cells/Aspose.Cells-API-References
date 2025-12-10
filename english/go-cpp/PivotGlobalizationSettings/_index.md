---
title: PivotGlobalizationSettings Class 
linktitle: PivotGlobalizationSettings
second_title: Aspose.Cells for Go via C++ API Reference
description: 'PivotGlobalizationSettings class. Encapsulates the object that represents pivotglobalizationsettings in Go.'
type: docs
weight: 200
url: /go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Represents the globalization settings for pivot tables.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Default constructor. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetTextOfTotal](./gettextoftotal/) | Gets the text of "Total" label in the PivotTable.You need to override this method when the PivotTable contains two or more PivotFields in the data area. | 
|[GetTextOfGrandTotal](./gettextofgrandtotal/) | Gets the text of "Grand Total" label in the PivotTable. | 
|[GetTextOfMultipleItems](./gettextofmultipleitems/) | Gets the text of "(Multiple Items)" label in the PivotTable. | 
|[GetTextOfAll](./gettextofall/) | Gets the text of "(All)" label in the PivotTable. | 
|[GetTextOfProtectedName](./gettextofprotectedname/) | Gets the text for specified protected name. | 
|[GetTextOfColumnLabels](./gettextofcolumnlabels/) | Gets the text of "Column Labels" label in the PivotTable. | 
|[GetTextOfRowLabels](./gettextofrowlabels/) | Gets the text of "Row Labels" label in the PivotTable. | 
|[GetTextOfEmptyData](./gettextofemptydata/) | Gets the text of "(blank)" label in the PivotTable. | 
|[GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Gets the the text of the value area field header in the PivotTable. | 
|[GetShortTextOf12Months](./getshorttextof12months/) | Gets all short formatted string of 12 months. | 
|[GetTextOf4Quaters](./gettextof4quaters/) | Gets the local text of 4 Quaters. | 
|[GetTextOfYears](./gettextofyears/) | Gets the local text of "Years". | 
|[GetTextOfQuarters](./gettextofquarters/) | Get the local text of "Quarters". | 
|[GetTextOfMonths](./gettextofmonths/) | Gets the local text of "Months". | 
|[GetTextOfDays](./gettextofdays/) | Gets the local text of "Days". | 
|[GetTextOfHours](./gettextofhours/) | Gets the local text of "Hours". | 
|[GetTextOfMinutes](./gettextofminutes/) | Gets the local text of "Minutes". | 
|[GetTextOfSeconds](./gettextofseconds/) | Gets the local text of "Seconds" | 
|[GetTextOfRange](./gettextofrange/) | Gets the local text of "Range" | 
|[GetTextOfAllPeriods](./gettextofallperiods/) | Gets the local text of "All Periods" | 
|[GetTextOfSubTotal](./gettextofsubtotal/) | Gets the text of PivotFieldSubtotalType type in the PivotTable. | 
|[GetNameOfDataField](./getnameofdatafield/) | Gets the display name of data pivot field.The default format is "Sum Of Field". | 
