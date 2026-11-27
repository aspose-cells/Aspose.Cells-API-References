---
title: "Klass PivotTableFormatCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableFormatCollection klass. Representerar samlingen av format som tillämpas på PivotTable"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableformatcollection/
---
## PivotTableFormatCollection class

Representerar en samling av format som tillämpas på PivotTable.

```csharp
public class PivotTableFormatCollection : CollectionBase<PivotTableFormat>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.pivot/pivottableformatcollection/item/) { get; } | Hämtar formatet efter indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.pivot/pivottableformatcollection/add/)() | Lägg till en [`PivotTableFormat`](../pivottableformat/). |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PivotTableFormat, IComparer&lt;PivotTableFormat&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PivotTableFormat) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PivotTableFormat[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PivotTableFormat[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PivotTableFormat&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PivotTableFormat&gt;) |  |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format)(CellArea, Style) | Formaterar markerat område i PivotTable. |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format_1)(PivotArea, Style) | Formaterar markerat område i PivotTable. |
| [Format](../../aspose.cells.pivot/pivottableformatcollection/format/#format_2)(int, int, Style) | Formaterar cellen i pivottabellområdet |
| [FormatArea](../../aspose.cells.pivot/pivottableformatcollection/formatarea/)(PivotFieldType, int, PivotFieldSubtotalType, PivotTableSelectionType, bool, bool, Style) | Formaterar markerat område. |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PivotTableFormat, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PivotTableFormat, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableFormatCollectionDemo
    {
        public static void PivotTableFormatCollectionExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Lägg till en pivottabell i kalkylbladet
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Kom åt PivotTableFormatCollection
            PivotTableFormatCollection formatCollection = pivotTable.PivotFormats;

            // Lägg till ett format till samlingen
            int formatIndex = formatCollection.Add();
            PivotTableFormat pivotFormat = formatCollection[formatIndex];

            // Definiera formatområdet
            PivotTableFormat newFormat = formatCollection.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, new Style());

            // Ange stilen för formatet
            Style style = new Style();
            style.BackgroundColor = Color.LightBlue;
            newFormat.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("PivotTableFormatCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PivotTableFormat](../pivottableformat/)
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


