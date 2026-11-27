---
title: "Klass UnionRange"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.UnionRange-klass. Representerar unionområde"
type: docs
url: /sv/net/aspose.cells/unionrange/
---
## UnionRange class

Representerar unionområde.

```csharp
public class UnionRange : IEnumerable
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [CellCount](../../aspose.cells/unionrange/cellcount/) { get; } | Hämtar antalet celler i området. |
| [ColumnCount](../../aspose.cells/unionrange/columncount/) { get; } | Hämtar antalet rader i området. |
| [FirstColumn](../../aspose.cells/unionrange/firstcolumn/) { get; } | Hämtar indexet för den första kolumnen i området. |
| [FirstRow](../../aspose.cells/unionrange/firstrow/) { get; } | Hämtar indexet för den första raden i området. |
| [HasRange](../../aspose.cells/unionrange/hasrange/) { get; } | Indikerar om detta har ett område. |
| [Hyperlinks](../../aspose.cells/unionrange/hyperlinks/) { get; } | Hämtar alla hyperlänkar i området. |
| [Name](../../aspose.cells/unionrange/name/) { get; set; } | Hämtar eller anger namnet på området. |
| [RangeCount](../../aspose.cells/unionrange/rangecount/) { get; } | Hämtar antalet områden. |
| [Ranges](../../aspose.cells/unionrange/ranges/) { get; } | Hämtar alla unionområden. |
| [RefersTo](../../aspose.cells/unionrange/refersto/) { get; } | Hämtar vad området refererar till. |
| [RowCount](../../aspose.cells/unionrange/rowcount/) { get; } | Hämtar antalet rader i området. |
| [Value](../../aspose.cells/unionrange/value/) { get; set; } | Hämtar och anger värdena för området. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ApplyStyle](../../aspose.cells/unionrange/applystyle/)(Style, StyleFlag) | Tillämpar format för ett helt område. |
| [Copy](../../aspose.cells/unionrange/copy/)(UnionRange, PasteOptions) | Kopierar området med specialklistra in-alternativ. |
| [GetEnumerator](../../aspose.cells/unionrange/getenumerator/)() | Hämtar enumeratorn för celler i detta område. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect)(Range[]) | Skär med ett annat område. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_2)(string) | Skär med ett annat område. |
| [Intersect](../../aspose.cells/unionrange/intersect/#intersect_1)(UnionRange) | Skär med ett annat område. |
| [Merge](../../aspose.cells/unionrange/merge/)() | Kombinerar ett cellområde till en enda cell. |
| [PutValue](../../aspose.cells/unionrange/putvalue/)(string, bool, bool) | Sätter ett värde i området, om lämpligt konverteras värdet till en annan datatyp och cellens talformat återställs. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders)(CellBorderType, Color) | Ställer in konturkanterna runt ett cellområde med samma kantstil och färg. |
| [SetOutlineBorders](../../aspose.cells/unionrange/setoutlineborders/#setoutlineborders_1)(CellBorderType[], Color[]) | Ställer in konturkanter runt ett cellområde. |
| [SetStyle](../../aspose.cells/unionrange/setstyle/)(Style) | Ställer in stilen för området. |
| [Union](../../aspose.cells/unionrange/union/#union)(Range[]) | Förenar områdena. |
| [Union](../../aspose.cells/unionrange/union/#union_2)(string) | Förenar ett annat område. |
| [Union](../../aspose.cells/unionrange/union/#union_1)(UnionRange) | Förenar ett annat område. |
| [UnMerge](../../aspose.cells/unionrange/unmerge/)() | Avslår sammanslagna celler i detta område. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassUnionRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa ett unionområde med rätt API
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A10,C1:C10", 0);
            
            // Ange värde för hela unionområdet
            unionRange.Value = "Test";
            
            // Applicera stil på unionområdet
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            unionRange.ApplyStyle(style, new StyleFlag { All = true });
            
            // Spara arbetsboken
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


