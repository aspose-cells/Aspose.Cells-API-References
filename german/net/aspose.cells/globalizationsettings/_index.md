---
title: GlobalizationSettings
second_title: Aspose.Cells für .NET-API-Referenz
description: Stellt die Globalisierungseinstellungen dar.
type: docs
weight: 3620
url: /de/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Stellt die Globalisierungseinstellungen dar.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Constructor |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Holt oder setzt das Diagramm davon[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Ruft das Trennzeichen für die Elemente in den Zeilendaten des Arrays in der Formel ab. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Liefert das Trennzeichen für Liste, Funktionsparameter, ...usw. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Ruft das Trennzeichen für Zeilen in Array-Daten in der Formel ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Vergleicht zwei Zeichenfolgenwerte gemäß bestimmten Sortierregeln. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Ruft den Namen des Labels „(Alle)“ in der PivotTable ab. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Ruft den Anzeigestringwert für den booleschen Wert der Zelle ab |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Wandelt den String gemäß bestimmten Sortierregeln in ein vergleichbares Objekt um. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Ruft den Namen der Bezeichnung "Spaltenbeschriftungen" in der PivotTable ab. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Ruft den vom Gebietsschema abhängigen Kommentartitelnamen gemäß dem Kommentartiteltyp ab. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Ruft den Namen des Labels „(leer)“ in der PivotTable ab. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Ruft den Anzeigestringwert für den Fehlerwert der Zelle ab |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Ruft den Gesamtsummennamen der Funktion ab. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Ruft den vom Gebietsschema abhängigen Text für den eingebauten Namen gemäß dem angegebenen Standardtext ab. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Ruft den vom Gebietsschema abhängigen Funktionsnamen gemäß dem angegebenen Standardfunktionsnamen ab. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Ruft den Namen der Bezeichnung „(Mehrere Elemente)“ in der PivotTable ab. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Ruft den Namen von "Anderen" Beschriftungen für Kreisdiagramme ab. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Ruft den Namen der Bezeichnung „Gesamtsumme“ in der PivotTable ab. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Ruft den Namen der Bezeichnung „Gesamt“ in der PivotTable ab. Sie müssen diese Methode überschreiben, wenn die PivotTable zwei oder mehr PivotFields im Datenbereich enthält. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Ruft den Schutznamen in der PivotTable ab. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Ruft den Namen der Beschriftung „Zeilenbeschriftungen“ in der PivotTable ab. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Ruft den Standardtext des eingebauten Namens gemäß dem gegebenen Gebietsschema-abhängigen Text ab. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Ruft den Standardfunktionsnamen gemäß dem angegebenen gebietsschemaabhängigen Funktionsnamen ab. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Ruft den standardmäßigen englischen Schriftstilnamen (regulär, fett, kursiv) für die Kopf-/Fußzeile gemäß dem gegebenen Gebietsschema-Schriftstilnamen ab. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Ruft den Namen von ab[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) Geben Sie die PivotTable ein. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Ruft den Typnamen von Tabellenzeilen ab, die aus allen Zeilen in der referenzierten Tabelle bestehen. Der Standardwert ist "Alle", sodass in der Formel "#All" alle Zeilen in der referenzierten Tabelle darstellt. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Ruft den Typnamen der Tabellenzeilen ab, die aus der aktuellen Zeile in der referenzierten Tabelle bestehen. Der Standardwert ist „Diese Zeile“, sodass in der Formel „#Diese Zeile“ die aktuelle Zeile in der referenzierten Tabelle darstellt. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Ruft den Typnamen von Tabellenzeilen ab, die aus dem Datenbereich der referenzierten Tabelle bestehen. Der Standardwert ist „Data“, also repräsentiert „#Data“ in der Formel den Datenbereich der Tabelle. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Ruft den Typnamen von Tabellenzeilen ab, der aus dem Tabellenkopf besteht. Der Standardwert ist "Kopfzeilen", also repräsentiert "#Kopfzeilen" in der Formel den Tabellenkopf. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Ruft den Typnamen von Tabellenzeilen ab, die aus der Gesamtzeile der referenzierten Tabelle bestehen. Der Standardwert ist "Totals", sodass in der Formel "#Totals" die Gesamtzeile der referenzierten Tabelle darstellt. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Ruft den Gesamtnamen der Funktion ab. |

### Siehe auch

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* namensraum [Aspose.Cells](../../aspose.cells)
* Montage [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
