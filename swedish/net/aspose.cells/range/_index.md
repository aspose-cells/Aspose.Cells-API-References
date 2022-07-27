---
title: Range
second_title: Aspose.Cells för .NET API-referens
description: Kapslar in objektet som representerar ett cellområde i ett kalkylblad.
type: docs
weight: 5030
url: /sv/net/aspose.cells/range/
---
## Range class

Kapslar in objektet som representerar ett cellområde i ett kalkylblad.

```csharp
public class Range
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Hämtar adressen till intervallet. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Hämtar antalet kolumner i intervallet. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Ställer in eller hämtar kolumnbredden för detta intervall |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Returnerar ett Range-objekt som representerar den aktuella regionen. Den aktuella regionen är ett intervall som begränsas av valfri kombination av tomma rader och tomma kolumner. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Hämtar ett Range-objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna intervallet. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Hämtar ett Range-objekt som representerar hela raden (eller raderna) som innehåller det angivna intervallet. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Hämtar indexet för den första kolumnen i intervallet. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Hämtar indexet för den första raden i intervallet. |
| [Height](../../aspose.cells/range/height) { get; } | Får bredden på ett intervall i punkter. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Får alla hyperlänkar i intervallet. |
| [Item](../../aspose.cells/range/item) { get; } | Blir[`Cell`](../cell) objekt i detta intervall. |
| [Left](../../aspose.cells/range/left) { get; } | Hämtar avståndet, i poäng, från den vänstra kanten av kolumn A till den vänstra kanten av intervallet. |
| [Name](../../aspose.cells/range/name) { get; set; } | Hämtar eller ställer in namnet på intervallet. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Hämtar intervallets referenser. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Hämtar antalet rader i intervallet. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Ställer in eller hämtar höjden på rader i detta intervall |
| [Top](../../aspose.cells/range/top) { get; } | Hämtar avståndet, i poäng, från den övre kanten av rad 1 till den övre kanten av intervallet. |
| [Value](../../aspose.cells/range/value) { get; set; } | Hämtar och ställer in värdet på intervallet. |
| [Width](../../aspose.cells/range/width) { get; } | Får bredden på ett intervall i punkter. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Får[`Worksheet`](./worksheet) objekt som innehåller detta intervall. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Tillämpar format för ett helt intervall. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Fyller automatiskt målintervallet. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Fyller automatiskt målintervallet. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källintervall. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Kopiera intervallet med specialalternativ för klistra in. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Kopierar celldata (inklusive formler) från ett källintervall. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Kopierar stilinställningar från ett källområde. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Kopierar cellvärde från ett källintervall. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Exporterar data i detta intervall till enDataTable objekt. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Exporterar data i detta intervall till enDataTable objekt. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Exporterar data i detta intervall till enDataTable objekt. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Blir[`Cell`](../cell) objekt eller null i detta intervall. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Hämtar enumeratorn för celler i detta intervall. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Blir[`Range`](../range) intervall med offset. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Returnerar en[`Range`](../range) objekt som representerar den rektangulära skärningspunkten mellan två områden. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Indikerar om området är skärande. |
| [Merge](../../aspose.cells/range/merge)() | Kombinerar ett cellintervall till en enda cell. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Flytta det aktuella intervallet till målintervallet. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Lägger ett värde i intervallet, om så är lämpligt kommer värdet att konverteras till annan datatyp och cellens talformat återställs. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Ange innanför gränserna för intervallet. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Anger konturkant runt ett cellintervall. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Ställer in konturkanterna runt ett cellintervall med samma kantstil och färg. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Anger linjekanter runt ett cellintervall. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Ställer in stilen för området. |
| override [ToString](../../aspose.cells/range/tostring)() | Returnerar en sträng som representerar det aktuella Range-objektet. |
| [Union](../../aspose.cells/range/union)(Range) | Returnerar föreningen av två intervall. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Tar bort sammanslagna celler i detta intervall. |

### Exempel

```csharp

[C#]

//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
// Få de första kalkylbladscellerna.
Cells cells = workbook.Worksheets[0].Cells;
// Skapa ett intervall (A1:D3).
Range range = cells.CreateRange("A1", "D3");
// Ställ in värdet på intervallet.
range.Value = "Hello";
//Spara Excel-filen
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiera ett arbetsboksobjekt
Dim workbook As Workbook = New Workbook()
'Skaffa de första kalkylbladscellerna.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Skapa ett intervall (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Ställ in värdet på intervallet.
range.Value = "Hello"
'Spara Excel-filen
workbook.Save("book1.xlsm")
```

### Se även

* namnutrymme [Aspose.Cells](../../aspose.cells)
* hopsättning [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
