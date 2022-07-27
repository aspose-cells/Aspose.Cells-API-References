---
title: GlobalizationSettings
second_title: Aspose.Cells för .NET API-referens
description: Representerar globaliseringsinställningarna.
type: docs
weight: 3620
url: /sv/net/aspose.cells/globalizationsettings/
---
## GlobalizationSettings class

Representerar globaliseringsinställningarna.

```csharp
public class GlobalizationSettings : AbstractGlobalizationSettings
```

## Konstruktörer

| namn | Beskrivning |
| --- | --- |
| [GlobalizationSettings](globalizationsettings)() | Default_Constructor |

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [ChartSettings](../../aspose.cells/globalizationsettings/chartsettings) { get; set; } | Hämtar eller ställer in diagrammet för detta[`ChartGlobalizationSettings`](../../aspose.cells.charts/chartglobalizationsettings) |
| virtual [ColumnSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/columnseparatorofformulaarray) { get; } | Hämtar avgränsaren för objekten i arrayens raddata i formel. |
| virtual [ListSeparator](../../aspose.cells/globalizationsettings/listseparator) { get; } | Hämtar avgränsaren för lista, funktionsparametrar, ...etc. |
| virtual [RowSeparatorOfFormulaArray](../../aspose.cells/globalizationsettings/rowseparatorofformulaarray) { get; } | Hämtar avgränsaren för rader i matrisdata i formel. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| virtual [Compare](../../aspose.cells/abstractglobalizationsettings/compare)(string, string, bool) | Jämför två strängvärden enligt vissa sorteringsregler. |
| virtual [GetAllName](../../aspose.cells/globalizationsettings/getallname)() | Hämtar namnet på etiketten "(Alla)" i pivottabellen. |
| virtual [GetBooleanValueString](../../aspose.cells/globalizationsettings/getbooleanvaluestring)(bool) | Hämtar visningssträngvärdet för cellens booleska värde |
| virtual [GetCollationKey](../../aspose.cells/abstractglobalizationsettings/getcollationkey)(string, bool) | Omvandlar strängen till ett jämförbart objekt enligt vissa sorteringsregler. |
| virtual [GetColumnLabelsOfPivotTable](../../aspose.cells/globalizationsettings/getcolumnlabelsofpivottable)() | Hämtar namnet på "kolumnetiketter" i pivottabellen. |
| virtual [GetCommentTitleName](../../aspose.cells/globalizationsettings/getcommenttitlename)(CommentTitleType) | Hämtar det språkberoende namnet på kommentarens titel enligt kommentarens titeltyp. |
| virtual [GetEmptyDataName](../../aspose.cells/globalizationsettings/getemptydataname)() | Hämtar namnet på etiketten "(tom)" i pivottabellen. |
| virtual [GetErrorValueString](../../aspose.cells/globalizationsettings/geterrorvaluestring)(string) | Hämtar visningssträngvärdet för cellens felvärde |
| virtual [GetGrandTotalName](../../aspose.cells/globalizationsettings/getgrandtotalname)(ConsolidationFunction) | Får det totala namnet på funktionen. |
| virtual [GetLocalBuiltInName](../../aspose.cells/globalizationsettings/getlocalbuiltinname)(string) | Hämtar den språkberoende texten för inbyggt Namn enligt given standardtext. |
| virtual [GetLocalFunctionName](../../aspose.cells/globalizationsettings/getlocalfunctionname)(string) | Hämtar det språkberoende funktionsnamnet enligt givet standardfunktionsnamn. |
| virtual [GetMultipleItemsName](../../aspose.cells/globalizationsettings/getmultipleitemsname)() | Hämtar namnet på etiketten "(Flera objekt)" i pivottabellen. |
| virtual [GetOtherName](../../aspose.cells/globalizationsettings/getothername)() | Hämtar namnet på "Andra"-etiketter för cirkeldiagram. |
| virtual [GetPivotGrandTotalName](../../aspose.cells/globalizationsettings/getpivotgrandtotalname)() | Hämtar namnet på etiketten "Grand Summa" i pivottabellen. |
| virtual [GetPivotTotalName](../../aspose.cells/globalizationsettings/getpivottotalname)() | Hämtar namnet på "Total"-etiketten i pivottabellen. Du måste åsidosätta denna metod när pivottabellen innehåller två eller flera pivotfält i dataområdet. |
| virtual [GetProtectionNameOfPivotTable](../../aspose.cells/globalizationsettings/getprotectionnameofpivottable)() | Hämtar skyddsnamnet i pivottabellen. |
| virtual [GetRowLabelsNameOfPivotTable](../../aspose.cells/globalizationsettings/getrowlabelsnameofpivottable)() | Hämtar namnet på etiketten "Radetiketter" i pivottabellen. |
| virtual [GetStandardBuiltInName](../../aspose.cells/globalizationsettings/getstandardbuiltinname)(string) | Hämtar standardtexten för inbyggt Namn enligt given språkberoende text. |
| virtual [GetStandardFunctionName](../../aspose.cells/globalizationsettings/getstandardfunctionname)(string) | Hämtar standardfunktionsnamnet enligt givet språkberoende funktionsnamn. |
| virtual [GetStandardHeaderFooterFontStyleName](../../aspose.cells/globalizationsettings/getstandardheaderfooterfontstylename)(string) | Får standardnamn för engelska teckensnittsstil (vanlig, fet, kursiv) för sidhuvud/sidfot enligt det givna språknamnet för teckensnittsstil. |
| virtual [GetSubTotalName](../../aspose.cells/globalizationsettings/getsubtotalname)(PivotFieldSubtotalType) | Får namnet på[`PivotFieldSubtotalType`](../../aspose.cells.pivot/pivotfieldsubtotaltype) skriv in pivottabellen. |
| virtual [GetTableRowTypeOfAll](../../aspose.cells/globalizationsettings/gettablerowtypeofall)() | Hämtar typnamnet på tabellrader som består av alla rader i den refererade tabellen. Standard är "Alla", så i formeln representerar "#All" alla rader i den refererade tabellen. |
| virtual [GetTableRowTypeOfCurrent](../../aspose.cells/globalizationsettings/gettablerowtypeofcurrent)() | Hämtar typnamnet på tabellrader som består av den aktuella raden i den refererade tabellen. Standard är "This Row", så i formeln representerar "#This Row" den aktuella raden i den refererade tabellen. |
| virtual [GetTableRowTypeOfData](../../aspose.cells/globalizationsettings/gettablerowtypeofdata)() | Hämtar typnamnet på tabellrader som består av dataregionen för den refererade tabellen. Standard är "Data", så i formeln representerar "#Data" dataregionen i tabellen. |
| virtual [GetTableRowTypeOfHeaders](../../aspose.cells/globalizationsettings/gettablerowtypeofheaders)() | Hämtar typnamnet på tabellrader som består av tabellhuvudet. Standard är "Headers", så i formeln representerar "#Headers" tabellhuvudet. |
| virtual [GetTableRowTypeOfTotals](../../aspose.cells/globalizationsettings/gettablerowtypeoftotals)() | Hämtar typnamnet på tabellrader som består av den totala raden av refererade tabeller. Standard är "Totals", så i formeln representerar "#Totals" den totala raden av refererade tabeller. |
| virtual [GetTotalName](../../aspose.cells/globalizationsettings/gettotalname)(ConsolidationFunction) | Får det totala namnet på funktionen. |

### Se även

* class [AbstractGlobalizationSettings](../abstractglobalizationsettings)
* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
