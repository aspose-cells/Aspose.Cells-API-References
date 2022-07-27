---
title: SeriesCollection
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Incapsula una raccolta diSeries./series oggetti.
type: docs
weight: 830
url: /it/net/aspose.cells.charts/seriescollection/
---
## SeriesCollection class

Incapsula una raccolta di[`Series`](../series) oggetti.

```csharp
public class SeriesCollection : CollectionBase<Series>
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase`1/capacity) { get; set; } |  |
| [CategoryData](../../aspose.cells.charts/seriescollection/categorydata) { get; set; } | Ottiene o imposta l'intervallo dei valori dell'asse della categoria. Può essere un intervallo di celle (come "d1:e10"), o una sequenza di valori (come "{2,6,8,10}"). |
| [Count](../../aspose.cells/collectionbase`1/count) { get; } |  |
| [IsColorVaried](../../aspose.cells.charts/seriescollection/iscolorvaried) { get; set; } | Rappresenta se il colore dei punti è variato. |
| [Item](../../aspose.cells.charts/seriescollection/item) { get; } | Ottiene il[`Series`](../series) elemento all'indice specificato. |
| [Item](../../aspose.cells/collectionbase`1/item) { get; set; } |  |
| [SecondCategoryData](../../aspose.cells.charts/seriescollection/secondcategorydata) { get; set; } | Ottiene o imposta l'intervallo dei valori dell'asse della seconda categoria. Può essere un intervallo di celle (come "d1:e10"), o una sequenza di valori (come "{2,6,8,10}"). Effetti solo quando alcune serie A vengono tracciate sul secondo asse. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Add](../../aspose.cells.charts/seriescollection/add#add)(string, bool) | Aggiunge il[`SeriesCollection`](../seriescollection) raccolta in un grafico. |
| [Add](../../aspose.cells.charts/seriescollection/add#add_1)(string, bool, bool) | Aggiunge il[`SeriesCollection`](../seriescollection) raccolta in un grafico. |
| [AddR1C1](../../aspose.cells.charts/seriescollection/addr1c1)(string, bool) | Aggiunge il[`SeriesCollection`](../seriescollection) raccolta in un grafico. |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(Series, IComparer&lt;Series&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase`1/binarysearch)(int, int, Series, IComparer&lt;Series&gt;) |  |
| [ChangeSeriesOrder](../../aspose.cells.charts/seriescollection/changeseriesorder)(int, int) | Modifica direttamente gli ordini delle due serie. |
| [Clear](../../aspose.cells.charts/seriescollection/clear#clear)() | Cancella la raccolta (2 methods) |
| [Contains](../../aspose.cells/collectionbase`1/contains)(Series) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[]) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(Series[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase`1/copyto)(int, Series[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase`1/exists)(Predicate&lt;Series&gt;) |  |
| [Find](../../aspose.cells/collectionbase`1/find)(Predicate&lt;Series&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase`1/findall)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, Predicate&lt;Series&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase`1/findindex)(int, int, Predicate&lt;Series&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase`1/findlast)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, Predicate&lt;Series&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase`1/findlastindex)(int, int, Predicate&lt;Series&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase`1/getenumerator)() |  |
| [GetSeriesByOrder](../../aspose.cells.charts/seriescollection/getseriesbyorder)(int) | Ottiene il[`Series`](../series) elemento per ordine. |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int) |  |
| [IndexOf](../../aspose.cells/collectionbase`1/indexof)(Series, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase`1/lastindexof)(Series, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/seriescollection/removeat#removeat)(int) | Rimuovi in una serie nell'indice specifico. (2 methods) |
| [SetSeriesNames](../../aspose.cells.charts/seriescollection/setseriesnames)(int, string, bool) | Imposta il nome di tutte le serie nel grafico. |

### Esempi

```csharp

[C#]
//Creazione di un'istanza di un oggetto cartella di lavoro
Workbook workbook = new Workbook();
//Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
int sheetIndex = workbook.Worksheets.Add();
//Ottenere il riferimento del foglio di lavoro appena aggiunto passando il relativo indice del foglio
Worksheet worksheet = workbook.Worksheets[sheetIndex];
//Aggiunta di un valore di esempio alla cella "A1".
worksheet.Cells["A1"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "A2".
worksheet.Cells["A2"].PutValue(100);
//Aggiunta di un valore di esempio alla cella "A3".
worksheet.Cells["A3"].PutValue(150);
//Aggiunta di un valore di esempio alla cella "A4".
worksheet.Cells["A4"].PutValue(200);
//Aggiunta di un valore di esempio alla cella "B1".
worksheet.Cells["B1"].PutValue(60);
//Aggiunta di un valore di esempio alla cella "B2".
worksheet.Cells["B2"].PutValue(32);
//Aggiunta di un valore di esempio alla cella "B3".
worksheet.Cells["B3"].PutValue(50);
//Aggiunta di un valore di esempio alla cella "B4".
worksheet.Cells["B4"].PutValue(40);
//Aggiunta di un valore di esempio alla cella "C1" come dati di categoria
worksheet.Cells["C1"].PutValue("Q1");
//Aggiunta di un valore di esempio alla cella "C2" come dati di categoria
worksheet.Cells["C2"].PutValue("Q2");
//Aggiunta di un valore di esempio alla cella "C3" come dati di categoria
worksheet.Cells["C3"].PutValue("Y1");
//Aggiunta di un valore di esempio alla cella "C4" come dati di categoria
worksheet.Cells["C4"].PutValue("Y2");
//Aggiunta di un grafico al foglio di lavoro
int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
//Accesso all'istanza del grafico appena aggiunto
Chart chart = worksheet.Charts[chartIndex];
//Aggiunta di NSeries (origine dati grafico) al grafico che va dalla cella "A1" a "B4"
chart.NSeries.Add("A1:B4", true);
//Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4";
//Salvataggio del file Excel
workbook.Save("book1.xls");

[Visual Basic]

'Creazione di un'istanza di un oggetto Workbook
Dim workbook As Workbook = New Workbook()
'Aggiunta di un nuovo foglio di lavoro all'oggetto Excel
Dim sheetIndex As Integer = workbook.Worksheets.Add()
'Ottenere il riferimento del foglio di lavoro appena aggiunto passando il suo indice del foglio
Dim worksheet As Worksheet = workbook.Worksheets(sheetIndex)
'Adding a sample value to "A1" cell
worksheet.Cells("A1").PutValue(50)
'Adding a sample value to "A2" cell
worksheet.Cells("A2").PutValue(100)
'Adding a sample value to "A3" cell
worksheet.Cells("A3").PutValue(150)
'Adding a sample value to "A4" cell
worksheet.Cells("A4").PutValue(200)
'Adding a sample value to "B1" cell
worksheet.Cells("B1").PutValue(60)
'Adding a sample value to "B2" cell
worksheet.Cells("B2").PutValue(32)
'Adding a sample value to "B3" cell
worksheet.Cells("B3").PutValue(50)
'Adding a sample value to "B4" cell
worksheet.Cells("B4").PutValue(40)
'Adding a sample value to "C1" cell as category data
worksheet.Cells("C1").PutValue("Q1")
'Adding a sample value to "C2" cell as category data
worksheet.Cells("C2").PutValue("Q2")
'Adding a sample value to "C3" cell as category data
worksheet.Cells("C3").PutValue("Y1")
'Adding a sample value to "C4" cell as category data
worksheet.Cells("C4").PutValue("Y2")
'Aggiunta di un grafico al foglio di lavoro
Dim chartIndex As Integer = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5)
'Accesso all'istanza del grafico appena aggiunto
Dim chart As Chart = worksheet.Charts(chartIndex)
'Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.NSeries.Add("A1:B4", True)
'Impostazione dell'origine dati per i dati di categoria di NSeries
chart.NSeries.CategoryData = "C1:C4"
'Salvataggio del file Excel
workbook.Save("book1.xls")
```

### Guarda anche

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1)
* class [Series](../series)
* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
