---
title: "GlobalizationSettings klass"
linktitle: "GlobalizationSettings"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "GlobalizationSettings-klass. Inkapslar objektet som representerar globalizationsettings i Go."
type: docs
weight: 200
url: /sv/go-cpp/globalizationsettings/
---

## GlobalizationSettings class

Representerar globaliseringsinställningarna.

```go

type GlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewGlobalizationSettings](./newglobalizationsettings/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetChartSettings](./getchartsettings/) | Hämtar globaliseringsinställningarna för diagram. |
| [SetChartSettings](./setchartsettings/) | Ställer in globaliseringsinställningarna för diagram. |
| [GetPivotSettings](./getpivotsettings/) | Hämtar globaliseringsinställningarna för pivottabell. |
| [SetPivotSettings](./setpivotsettings/) | Ställer in globaliseringsinställningarna för pivottabell. |
| [GetTotalName](./gettotalname/) | Hämtar det totala namnet på funktionen. |
| [GetGrandTotalName](./getgrandtotalname/) | Hämtar det övergripande totalsnamnet för funktionen. |
| [GetDefaultSheetName](./getdefaultsheetname/) | Hämtar standardnamnet på bladet för att automatiskt lägga till ett kalkylblad. Standard är "Sheet". |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Hämtar typnamnet för tabellrader som består av datasektionen i den refererade tabellen. Standard är "Data", så i formeln "#Data" representerar datasektionen i tabellen. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. Standard är "All", så i formeln "#All" representerar alla rader i den refererade tabellen. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. Standard är "Totals", så i formeln "#Totals" representerar totalraden i den refererade tabellen. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. Standard är "This Row", så i formeln "#This Row" representerar den aktuella raden i den refererade tabellen. |
| [GetErrorValueString](./geterrorvaluestring/) | Hämtar displaysträngvärdet för cellens felvärde |
| [GetBooleanValueString](./getbooleanvaluestring/) | Hämtar displaysträngvärdet för cellens booleska värde |
| [GetLocalFunctionName](./getlocalfunctionname/) | Hämtar det localespecifika funktionsnamnet enligt angivet standardfunktionsnamn. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Hämtar standardfunktionsnamnet enligt angivet localespecifikt funktionsnamn. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Hämtar den localespecifika texten för inbyggt namn enligt angiven standardtext. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Hämtar standardtexten för inbyggt namn enligt given localespecifik text. |
| [GetListSeparator](./getlistseparator/) | Hämtar avgränsaren för lista, parametrar för funktion, ...etc. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Hämtar avgränsaren för rader i matrisdata i formeln. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Hämtar avgränsaren för objekten i matrisens raddata i formeln. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Hämtar standardengelskt typsnittsstilsnamn (Regular, Bold, Italic) för sidhuvud/sidfot enligt angivet localespecifikt typsnittsstilsnamn. |
| [GetCommentTitleName](./getcommenttitlename/) | Hämtar den localespecifika kommentarsrubrikens namn enligt kommentarsrubriktyp. |
| [Compare](./compare/) | Jämför två strängvärden enligt vissa sorteringsregler. |
