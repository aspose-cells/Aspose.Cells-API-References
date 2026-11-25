---
title: "Classe SeriesCollection"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.SeriesCollection. Incapsula una raccolta di oggetti Series"
type: docs
url: /it/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Incapsula una raccolta di oggetti [`Series`](../series/).

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata/) { get; set; } | Ottiene o imposta l'intervallo dei valori dell'asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10") o una sequenza di valori (ad esempio "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried/) { get; set; } | Rappresenta se il colore dei punti è variabile. |
| [Item](../../aspose.cells.charts/seriescollection/item/) { get; } | Ottiene l'elemento [`Series`](../series/) all'indice specificato. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata/) { get; set; } | Ottiene o imposta l'intervallo dei valori del secondo asse di categoria. Può essere un intervallo di celle (ad esempio "d1:e10"), o una sequenza di valori (ad esempio "{2,6,8,10}"). Ha effetto solo quando alcune serie sono tracciate sul secondo asse. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add/#add)(string, bool) | Aggiunge la raccolta [`Series`](../series/) a un grafico. |
| [Add](../../aspose.cells.charts/seriescollection/add/#add_1)(string, bool, bool) | Aggiunge la raccolta [`Series`](../series/) a un grafico. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1/)(string, bool) | Aggiunge la raccolta [`Series`](../series/) a un grafico. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeColors](../../aspose.cells.charts/seriescollection/changecolors/)(ChartColorPaletteType) | Imposta la palette monocromatica per le serie del grafico. |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder/)(int, int) | (**Obsolete.**) Cambia direttamente l'ordine delle due serie. |
| [Clear](../../aspose.cells.charts/seriescollection/clear/#clear)() | Cancella la raccolta (2 metodi) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder/)(int) | Ottiene l'elemento [`Series`](../series/) per ordine. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat/#removeat)(int) | Rimuove una serie all'indice specifico. (2 metodi) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames/)(int, string, bool) | Imposta i nomi di tutte le serie nel grafico. |
| [SwapSeries](../../aspose.cells.charts/seriescollection/swapseries/)(int, int) | Cambia direttamente l'ordine delle due serie. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SeriesCollectionDemo
    {
        public static void SeriesCollectionExample()
        {
            // Istanziare un oggetto Workbook
            Workbook workbook = new Workbook();
            
            // Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice di foglio
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Aggiunta di valori di esempio alle celle
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Aggiunta di un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accesso all'istanza del grafico appena aggiunto
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiunta di NSeries (origine dati del grafico) al grafico che va dalla cella "A1" alla "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Impostazione dell'origine dati per i dati di categoria di NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Accesso alla SeriesCollection del grafico
            SeriesCollection seriesCollection = chart.NSeries;

            // Impostazione delle proprietà della SeriesCollection
            seriesCollection.CategoryData = "C1:C4";
            seriesCollection.SecondCategoryData = "C1:C4";
            seriesCollection.IsColorVaried = true;

            // Accesso a una serie specifica nella SeriesCollection
            Series series = seriesCollection[0];
            
            // Impostazione delle proprietà della serie
            series.Values = "=B1:B4";
            series.Name = "First Series";
            series.Type = ChartType.Line;
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;

            // Salvataggio del file Excel
            workbook.Save("SeriesCollectionExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Series](../series/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


