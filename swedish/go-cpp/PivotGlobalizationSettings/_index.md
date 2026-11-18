---
title: "PivotGlobalizationSettings-klass"
linktitle: "PivotGlobalizationSettings"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "PivotGlobalizationSettings-klass. Inkapslar objektet som representerar pivotglobalizationsettings i Go."
type: docs
weight: 200
url: /sv/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Representerar globaliseringsinställningarna för pivottabeller.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetTextOfTotal](./gettextoftotal/) | Hämtar texten för etiketten "Total" i PivotTable. Du måste åsidosätta den här metoden när PivotTable innehåller två eller fler PivotFields i dataområdet. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Hämtar texten för etiketten "Grand Total" i PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Hämtar texten för etiketten "(Multiple Items)" i PivotTable. |
| [GetTextOfAll](./gettextofall/) | Hämtar texten för etiketten "(All)" i PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Hämtar texten för angivet skyddat namn. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Hämtar texten för etiketten "Column Labels" i PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Hämtar texten för "Row Labels"-etiketten i pivottabellen. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Hämtar texten för "(blank)"-etiketten i pivottabellen. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Hämtar texten för fältets rubrik i värdeområdet i pivottabellen. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Hämtar alla korta formaterade strängar för 12 månader. |
| [GetTextOf24Hours](./gettextof24hours/) | Hämtar alla lokalt formaterade strängar för 24 timmar.Standardvärdet är 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Hämtar alla lokalt formaterade strängar för "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Hämtar talformatet för pivottagsgrupp. Används endast när pivottfältet grupperas efter dagar. Standardvärdet är "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Hämtar den lokala texten för 4 kvartal. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Hämtar den lokala texten för 4 kvartal. |
| [GetTextOfYears](./gettextofyears/) | Hämtar den lokala texten för "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Hämtar den lokala texten för "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Hämtar den lokala texten för "Months". |
| [GetTextOfDays](./gettextofdays/) | Hämtar den lokala texten för "Days". |
| [GetTextOfHours](./gettextofhours/) | Hämtar den lokala texten för "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Hämtar den lokala texten för "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Hämtar den lokala texten för "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Hämtar den lokala texten för "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Hämtar den lokala texten för "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Hämtar texten för PivotFieldSubtotalType-typen i pivottabellen. |
| [GetNameOfDataField](./getnameofdatafield/) | Hämtar visningsnamnet för datapivottfältet. Standardformatet är "Sum Of Field". |
