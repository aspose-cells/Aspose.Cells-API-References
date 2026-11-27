---
title: "Klassen Range"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Range-klass. Inkapslar objektet som representerar ett cellområde i ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/range/
---
## Range class

Inkapslar objektet som representerar ett cellområde i ett kalkylblad.

```csharp
public class Range : IEnumerable
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Klasskonstruktor. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Klasskonstruktor. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Hämtar adressen för området. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Hämtar antalet kolumner i området. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Anger eller hämtar kolumnbredden för detta område |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Returnerar ett Range-objekt som representerar den aktuella regionen. Den aktuella regionen är ett område som begränsas av en kombination av tomma rader och tomma kolumner. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Hämtar ett Range-objekt som representerar hela kolumnen (eller kolumnerna) som innehåller det angivna området. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Hämtar ett Range-objekt som representerar hela raden (eller raderna) som innehåller det angivna området. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Hämtar indexet för den första kolumnen i området. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Hämtar indexet för den första raden i området. |
| [Height](../../aspose.cells/range/height/) { get; } | Hämtar bredden på ett område i punkter. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Hämtar alla hyperlänkar i området. |
| [Item](../../aspose.cells/range/item/) { get; } | Hämtar [`Cell`](../cell/) objekt i detta område. |
| [Left](../../aspose.cells/range/left/) { get; } | Hämtar avståndet, i punkter, från vänstra kanten av kolumn A till vänstra kanten av området. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Hämtar eller anger namnet på området. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Hämtar vad området refererar till. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Hämtar antalet rader i området. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Anger eller hämtar höjden på raderna i detta område |
| [Top](../../aspose.cells/range/top/) { get; } | Hämtar avståndet, i punkter, från överkanten av rad 1 till överkanten av området. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Hämtar och anger värdet för området. |
| [Width](../../aspose.cells/range/width/) { get; } | Hämtar bredden på ett område i punkter. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Hämtar [`Worksheet`](./worksheet/)objektet som innehåller detta område. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Lägger till en hyperlänk till en angiven cell eller ett cellområde. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Tillämpar format för ett helt område. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Fyller automatiskt målområdet. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Fyller automatiskt målområdet. |
| [Clear](../../aspose.cells/range/clear/)() | Rensar detta område. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Rensar kommentarerna i detta område. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Rensar innehållet i detta område. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Rensar formaten i detta område. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Tar bara bort hyperlänkar. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Kopierar data (inklusive formler), formatering, ritobjekt etc. från ett källområde. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Kopierar området med specialklistra in-alternativ. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Kopierar celldata (inklusive formler) från ett källområde. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Kopierar stilinställningar från ett källområde. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Kopierar cellvärde från ett källområde. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Exporterar data i detta område till ett DataTable-objekt. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Exporterar data i detta område till ett DataTable-objekt. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Exporterar data i detta område till ett DataTable-objekt. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Hämtar [`Cell`](../cell/)objektet eller null i detta område. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Hämtar enumeratorn för celler i detta område. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Hämtar `Range`-området med förskjutning. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Returnerar ett `Range`-objekt som representerar den rektangulära skärningen av två områden. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Anger om området innehåller värden. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Anger om området intersecteras. |
| [Merge](../../aspose.cells/range/merge/)() | Kombinerar ett cellområde till en enda cell. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Flyttar det aktuella området till destinationsområdet. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Sätter ett värde i området, om lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Ställ in inre kanter för området. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Ställer in konturkant runt ett cellområde. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Ställer in konturkant runt ett cellområde. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Ställer in konturkanterna runt ett cellområde med samma kantstil och färg. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Ställer in konturkanterna runt ett cellområde med samma kantstil och färg. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Ställer in konturkanter runt ett cellområde. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Ställer in stilen för området. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Applicera cellstilen. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Konvertera området till HTML. |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Konverterar området till en bild. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Konvertera området till JSON‑värde. |
| override [ToString](../../aspose.cells/range/tostring/)() | Returnerar en sträng som representerar det aktuella Range-objektet. |
| [Transpose](../../aspose.cells/range/transpose/)() | Transponera (rotera) data från rader till kolumner eller omvänt. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) Returnerar unionen av två områden. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) Returnerar unionsresultatet av två områden. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Returnerar unionsresultatet av två områden. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Avslår sammanslagna celler i detta område. |

### Anmärkningar

Range‑klassen betecknar en region i ett Excel‑kalkylblad. Med den kan du formatera och ange värdet för området. Och du kan också enkelt kopiera ett Excel‑område.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


