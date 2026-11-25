---
title: "Classe SparklineCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.SparklineCollection. Incapsula una raccolta di oggetti Sparkline"
type: docs
url: /it/net/aspose.cells.charts/sparklinecollection/
---
## SparklineCollection class

Incapsula una raccolta di oggetti [`Sparkline`](../sparkline/).

```csharp
public class SparklineCollection : CollectionBase<Sparkline>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinecollection/item/) { get; } | Restituisce l'elemento [`Sparkline`](../sparkline/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinecollection/add/)(string, int, int) | Aggiungi uno sparkline. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Sparkline) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Sparkline, IComparer&lt;Sparkline&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Sparkline, IComparer&lt;Sparkline&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Sparkline) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Sparkline[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Sparkline[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Sparkline[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Sparkline&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Sparkline&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Sparkline&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Sparkline&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Sparkline&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Sparkline&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Sparkline, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Sparkline, int, int) |  |
| [Remove](../../aspose.cells.charts/sparklinecollection/remove/)(object) | (**Obsoleto.**) Rimuove lo sparkline |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [RemoveSparkline](../../aspose.cells.charts/sparklinecollection/removesparkline/)(Sparkline) | Rimuove lo sparkline |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionDemo
    {
        public static void SparklineCollectionExample()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Inserisci dati di esempio nel foglio di lavoro
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);
            

            // Definisci il CellArea dove verranno aggiunti gli sparklines
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Aggiungi un nuovo SparklineGroup al foglio di lavoro
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;
            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Aggiungi sparklines al SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Imposta varie proprietà per il SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Imposta i colori per i punti alti e bassi
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Imposta il colore della serie e lo spessore della linea
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Sparkline](../sparkline/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


