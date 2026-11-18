---
title: "SettableGlobalizationSettings-klass"
linktitle: "SettableGlobalizationSettings"
second_title: "Aspose.Cells för Go via C++ API-referens"
description: "SettableGlobalizationSettings-klass. Inkapslar objektet som representerar settableglobalizationsettings i Go."
type: docs
weight: 200
url: /sv/go-cpp/settableglobalizationsettings/
---

## SettableGlobalizationSettings class

Implementering av GlobalizationSettings som låter användaren ange/ändra fördefinierade texter.

```go

type SettableGlobalizationSettings struct  {
	ptr unsafe.Pointer
}

```
## Konstruktörer

| Metod | Beskrivning |
| --- | --- |
| [NewSettableGlobalizationSettings](./newsettableglobalizationsettings/) | Standardkonstruktor. |

## Metoder

| Metod | Beskrivning |
| --- | --- |
| [IsNull](./isnull/) | Kontrollerar om implementeringsobjektet är nullptr. |
| [GetTotalName](./gettotalname/) | Hämtar det totala namnet på en specifik funktion. |
| [SetTotalName](./settotalname/) | Ställer in det totala namnet på en specifik funktion. |
| [GetGrandTotalName](./getgrandtotalname/) | Hämtar det övergripande totalsnamnet för funktionen. |
| [SetGrandTotalName](./setgrandtotalname/) | Ställer in det övergripande totalsnamnet för en specifik funktion. |
| [GetTableRowTypeOfHeaders](./gettablerowtypeofheaders/) | Hämtar typnamnet för tabellrader som består av tabellrubriken. Standard är "Headers", så i formeln "#Headers" representerar tabellrubriken. |
| [SetTableRowTypeOfHeaders](./settablerowtypeofheaders/) | Ställer in typnamnet för tabellrader som består av tabellrubriken. |
| [GetTableRowTypeOfData](./gettablerowtypeofdata/) | Hämtar typnamnet för tabellrader som består av datasektionen i den refererade tabellen. Standard är "Data", så i formeln "#Data" representerar datasektionen i tabellen. |
| [SetTableRowTypeOfData](./settablerowtypeofdata/) | Ställer in typnamnet för tabellrader som består av datasektionen i den refererade tabellen. |
| [GetTableRowTypeOfAll](./gettablerowtypeofall/) | Hämtar typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| [SetTableRowTypeOfAll](./settablerowtypeofall/) | Ställer in typnamnet för tabellrader som består av alla rader i den refererade tabellen. |
| [GetTableRowTypeOfTotals](./gettablerowtypeoftotals/) | Hämtar typnamnet för tabellrader som består av totalraden i den refererade tabellen. |
| [SetTableRowTypeOfTotals](./settablerowtypeoftotals/) | Ställer in typnamnet för tabellrader som består av totalraden i den refererade tabellen. |
| [GetTableRowTypeOfCurrent](./gettablerowtypeofcurrent/) | Hämtar typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| [SetTableRowTypeOfCurrent](./settablerowtypeofcurrent/) | Ställer in typnamnet för tabellrader som består av den aktuella raden i den refererade tabellen. |
| [GetErrorValueString](./geterrorvaluestring/) | Hämtar displaysträngvärdet för cellens felvärde |
| [GetBooleanValueString](./getbooleanvaluestring/) | Hämtar displaysträngvärdet för cellens booleska värde |
| [SetBooleanValueString](./setbooleanvaluestring/) | Ställer in displaysträngvärdet för cellens booleska värde |
| [GetLocalFunctionName](./getlocalfunctionname/) | Hämtar det localespecifika funktionsnamnet enligt angivet standardfunktionsnamn. |
| [SetLocalFunctionName](./setlocalfunctionname/) | Ställer in det localespecifika funktionsnamnet som motsvarar angivet standardfunktionsnamn. |
| [GetStandardFunctionName](./getstandardfunctionname/) | Hämtar standardfunktionsnamnet enligt angivet localespecifikt funktionsnamn. |
| [SetStandardFunctionName](./setstandardfunctionname/) | Ställer in det localespecifika funktionsnamnet enligt angivet standardfunktionsnamn. |
| [GetLocalBuiltInName](./getlocalbuiltinname/) | Hämtar den localespecifika texten för inbyggt namn enligt angiven standardtext. |
| [SetLocalBuiltInName](./setlocalbuiltinname/) | Ställer in den localespecifika texten för det inbyggda namnet med given standardnamntext. |
| [GetStandardBuiltInName](./getstandardbuiltinname/) | Hämtar standardtexten för inbyggt namn enligt given localespecifik text. |
| [SetStandardBuiltInName](./setstandardbuiltinname/) | Ställer in det localespecifika funktionsnamnet enligt angivet standardfunktionsnamn. |
| [GetListSeparator](./getlistseparator/) | Hämtar avgränsaren för lista, parametrar för funktion, ...etc. |
| [SetListSeparator](./setlistseparator/) | Ställer in avgränsaren för lista, parametrar för funktion, ...etc. |
| [GetRowSeparatorOfFormulaArray](./getrowseparatorofformulaarray/) | Hämtar avgränsaren för rader i matrisdata i formeln. |
| [SetRowSeparatorOfFormulaArray](./setrowseparatorofformulaarray/) | Ställer in avgränsaren för rader i matrisdata i formeln. |
| [GetColumnSeparatorOfFormulaArray](./getcolumnseparatorofformulaarray/) | Hämtar avgränsaren för objekten i matrisens raddata i formeln. |
| [SetColumnSeparatorOfFormulaArray](./setcolumnseparatorofformulaarray/) | Ställer in avgränsaren för objekten i matrisens raddata i formeln. |
| [GetStandardHeaderFooterFontStyleName](./getstandardheaderfooterfontstylename/) | Hämtar standardengelskt typsnittsstilsnamn (Regular, Bold, Italic) för sidhuvud/sidfot enligt angivet localespecifikt typsnittsstilsnamn. |
| [SetStandardHeaderFooterFontStyleName](./setstandardheaderfooterfontstylename/) | Ställer in det localespecifika funktionsnamnet enligt angivet standardfunktionsnamn. |
| [GetCommentTitleName](./getcommenttitlename/) | Hämtar den localespecifika kommentarsrubrikens namn enligt kommentarsrubriktyp. |
| [SetCommentTitleName](./setcommenttitlename/) | Hämtar den localespecifika kommentarsrubrikens namn enligt kommentarsrubriktyp. |
