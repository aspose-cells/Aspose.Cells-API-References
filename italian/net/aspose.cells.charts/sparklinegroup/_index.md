---
title: SparklineGroup
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Sparkline./sparkline è organizzato in un gruppo sparkline. Un SparklineGroup contiene un numero variabile di elementi sparkline. Un gruppo sparkline specifica il tipo le impostazioni di visualizzazione e le impostazioni degli assi per gli sparkline.
type: docs
weight: 880
url: /it/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline) è organizzato in un gruppo sparkline. Un SparklineGroup contiene un numero variabile di elementi sparkline. Un gruppo sparkline specifica il tipo, le impostazioni di visualizzazione e le impostazioni degli assi per gli sparkline.

```csharp
public class SparklineGroup
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden) { get; set; } | Indica se mostrare i dati in righe e colonne nascoste. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor) { get; set; } | Ottiene e imposta il colore del primo punto di dati nel gruppo sparkline. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor) { get; set; } | Ottiene e imposta il colore dei punti più alti dei dati nel gruppo sparkline. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor) { get; set; } | Ottiene e imposta il colore dell'asse orizzontale nel gruppo sparkline. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange) { get; set; } | Rappresenta l'intervallo che contiene i valori di data per i dati sparkline. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor) { get; set; } | Ottiene e imposta il colore dell'ultimo punto di dati nel gruppo sparkline. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight) { get; set; } | Ottiene e imposta lo spessore di linea in ciascuna linea sparkline nel gruppo sparkline, nell'unità di punti. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor) { get; set; } | Ottiene e imposta il colore dei punti più bassi dei dati nel gruppo sparkline. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor) { get; set; } | Ottiene e imposta il colore dei punti in ciascuna linea sparkline nel gruppo sparkline. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor) { get; set; } | Ottiene e imposta il colore dei valori negativi nel gruppo sparkline. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype) { get; set; } | Indica come tracciare le celle vuote. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft) { get; set; } | Indica se i dati del grafico sono da destra a sinistra. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle) { get; set; } | Ottiene e imposta il tipo di stile predefinito del gruppo sparkline. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor) { get; set; } | Ottiene e imposta il colore delle sparkline nel gruppo sparkline. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint) { get; set; } | Indica se evidenziare il primo punto di dati nel gruppo sparkline. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint) { get; set; } | Indica se evidenziare i punti più alti dei dati nel gruppo sparkline. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis) { get; set; } | Indica se visualizzare l'asse orizzontale della sparkline. L'asse orizzontale viene visualizzato se la sparkline ha dati che attraversano l'asse zero. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint) { get; set; } | Indica se evidenziare l'ultimo punto di dati nel gruppo sparkline. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint) { get; set; } | Indica se evidenziare i punti più bassi dei dati nel gruppo sparkline. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers) { get; set; } | Indica se evidenziare ogni punto in ogni linea sparkline nel gruppo sparkline. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints) { get; set; } | Indica se evidenziare i valori negativi sul gruppo sparkline con un colore o un indicatore diverso. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection) { get; } | Ottiene il[`SparklineCollection`](./sparklinecollection) oggetto del gruppo sparkline. |
| [Type](../../aspose.cells.charts/sparklinegroup/type) { get; set; } | Indica il tipo di sparkline del gruppo sparkline. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue) { get; set; } | Ottiene e imposta il valore massimo personalizzato per l'asse verticale. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype) { get; set; } | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue) { get; set; } | Ottiene e imposta il valore minimo personalizzato per l'asse verticale. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype) { get; set; } | Rappresenta il tipo di valore minimo dell'asse verticale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges)(string, bool, CellArea) | Reimposta l'intervallo di dati e l'intervallo di posizioni del gruppo sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli. |

### Esempi

```csharp
[C#]
 Workbook book = new Workbook(); 
 Worksheet sheet = book.Worksheets[0];

 sheet.Cells["A1"].PutValue(5);
 sheet.Cells["B1"].PutValue(2);
 sheet.Cells["C1"].PutValue(1);
 sheet.Cells["D1"].PutValue(3);
 
 // Definisci la CellArea
 CellArea ca = new CellArea();
 ca.StartColumn = 4;
 ca.EndColumn = 4;
 ca.StartRow = 0;
 ca.EndRow = 0;
 int idx = sheet.SparklineGroupCollection.Add(Aspose.Cells.Charts.SparklineType.Line, "A1:D1", false, ca);
 SparklineGroup group = sheet.SparklineGroupCollection[idx];
 group.SparklineCollection.Add(sheet.Name + "!A1:D1", 0, 4);
 // Crea CellsColor
 CellsColor clr = book.CreateCellsColor();
 clr.Color = Color.Orange;
 group.SeriesColor = clr;

 // imposta i punti alti sono colorati di verde e i punti bassi sono colorati di rosso
 group.ShowHighPoint = true;
 group.ShowLowPoint = true;
 group.HighPointColor.Color = Color.Green;
 group.LowPointColor.Color = Color.Red;
 // imposta lo spessore della linea 
 group.LineWeight = 1.0;
 book.Save("output.xlsx", SaveFormat.Xlsx);
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.Charts](../../aspose.cells.charts)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
