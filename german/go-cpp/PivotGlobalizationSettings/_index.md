---
title: "PivotGlobalizationSettings Klasse"
linktitle: "PivotGlobalizationSettings"
second_title: "Aspose.Cells für Go über C++‑API‑Referenz"
description: "PivotGlobalizationSettings Klasse. Kapselt das Objekt, das pivotglobalizationsettings in Go darstellt."
type: docs
weight: 200
url: /de/go-cpp/pivotglobalizationsettings/
---

## PivotGlobalizationSettings class

Stellt die Globalisierungseinstellungen für Pivot-Tabellen dar.

```go

type PivotGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktoren

| Methode | Beschreibung |
| --- | --- |
| [NewPivotGlobalizationSettings](./newpivotglobalizationsettings/) | Standardkonstruktor. |

## Methoden

| Methode | Beschreibung |
| --- | --- |
| [IsNull](./isnull/) | Überprüft, ob das Implementierungsobjekt nullptr ist. |
| [GetTextOfTotal](./gettextoftotal/) | Liefert den Text des "Total"-Labels in der PivotTable. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält. |
| [GetTextOfGrandTotal](./gettextofgrandtotal/) | Liefert den Text des "Grand Total"-Labels in der PivotTable. |
| [GetTextOfMultipleItems](./gettextofmultipleitems/) | Liefert den Text des "(Multiple Items)"-Labels in der PivotTable. |
| [GetTextOfAll](./gettextofall/) | Liefert den Text des "(All)"-Labels in der PivotTable. |
| [GetTextOfProtectedName](./gettextofprotectedname/) | Liefert den Text für den angegebenen geschützten Namen. |
| [GetTextOfColumnLabels](./gettextofcolumnlabels/) | Liefert den Text des "Column Labels"-Labels in der PivotTable. |
| [GetTextOfRowLabels](./gettextofrowlabels/) | Liefert den Text des "Row Labels"-Labels in der PivotTable. |
| [GetTextOfEmptyData](./gettextofemptydata/) | Liefert den Text des "(blank)"-Labels in der PivotTable. |
| [GetTextOfDataFieldHeader](./gettextofdatafieldheader/) | Liefert den Text der Feldkopfzeile des Wertebereichs in der PivotTable. |
| [GetShortTextOf12Months](./getshorttextof12months/) | Liefert alle kurz formatierten Zeichenketten von 12 Monaten. |
| [GetTextOf24Hours](./gettextof24hours/) | Liefert alle lokal formatierten Zeichenketten von 24 Stunden. Der Standardwert ist 12 AM, 1 AM, 2 AM, 3 AM, 4 AM, 5 AM, 6 AM, 7 AM, 8 AM, 9 AM, 10 AM, 11 AM, 12 PM, 1 PM, 2 PM, 3 PM, 4 PM, 5 PM, 6 PM, 7 PM, 8 PM, 9 PM, 10 PM, 11 PM. |
| [GetTextOfOr](./gettextofor/) | Liefert alle lokal formatierten Zeichenketten von "or". |
| [GetFormatOfDayGroup](./getformatofdaygroup/) | Liefert das Zahlenformat der Pivot‑Tag‑Gruppe. Wird nur verwendet, wenn das Pivot‑Feld nach Tagen gruppiert wird. Der Standardwert ist "d-MMM"; |
| [GetTextOf4Quaters](./gettextof4quaters/) | Liefert den lokalen Text von 4 Quartalen. |
| [GetTextOf4Quarters](./gettextof4quarters/) | Liefert den lokalen Text von 4 Quartalen. |
| [GetTextOfYears](./gettextofyears/) | Liefert den lokalen Text von "Years". |
| [GetTextOfQuarters](./gettextofquarters/) | Liefert den lokalen Text von "Quarters". |
| [GetTextOfMonths](./gettextofmonths/) | Liefert den lokalen Text von "Months". |
| [GetTextOfDays](./gettextofdays/) | Liefert den lokalen Text von "Days". |
| [GetTextOfHours](./gettextofhours/) | Liefert den lokalen Text von "Hours". |
| [GetTextOfMinutes](./gettextofminutes/) | Liefert den lokalen Text von "Minutes". |
| [GetTextOfSeconds](./gettextofseconds/) | Liefert den lokalen Text von "Seconds" |
| [GetTextOfRange](./gettextofrange/) | Liefert den lokalen Text von "Range" |
| [GetTextOfAllPeriods](./gettextofallperiods/) | Liefert den lokalen Text von "All Periods" |
| [GetTextOfSubTotal](./gettextofsubtotal/) | Liefert den Text des PivotFieldSubtotalType-Typs in der PivotTable. |
| [GetNameOfDataField](./getnameofdatafield/) | Liefert den Anzeigenamen des Daten-Pivotfelds. Das Standardformat ist "Sum Of Field". |
