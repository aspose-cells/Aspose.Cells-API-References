---
title: "Classe SparklineGroup"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.SparklineGroup. Sparkline è organizzato in un gruppo di sparkline. Un SparklineGroup contiene un numero variabile di elementi sparkline. Un gruppo di sparkline specifica le impostazioni di visualizzazione del tipo e le impostazioni dell'asse per le sparkline."
type: docs
url: /it/net/aspose.cells.charts/sparklinegroup/
---
## SparklineGroup class

[`Sparkline`](../sparkline/) is organized into a sparkline group. A SparklineGroup contains a variable number of sparkline items. A sparkline group specifies the type, display settings and axis settings for the sparklines.

```csharp
public class SparklineGroup
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DisplayHidden](../../aspose.cells.charts/sparklinegroup/displayhidden/) { get; set; } | Indica se mostrare i dati in righe e colonne nascoste. |
| [FirstPointColor](../../aspose.cells.charts/sparklinegroup/firstpointcolor/) { get; set; } | Ottiene e imposta il colore del primo punto dati nel gruppo di sparkline. |
| [HighPointColor](../../aspose.cells.charts/sparklinegroup/highpointcolor/) { get; set; } | Ottiene e imposta il colore dei punti più alti dei dati nel gruppo di sparkline. |
| [HorizontalAxisColor](../../aspose.cells.charts/sparklinegroup/horizontalaxiscolor/) { get; set; } | Ottiene e imposta il colore dell'asse orizzontale nel gruppo di sparkline. |
| [HorizontalAxisDateRange](../../aspose.cells.charts/sparklinegroup/horizontalaxisdaterange/) { get; set; } | Rappresenta l'intervallo che contiene i valori di data per i dati della sparkline. |
| [LastPointColor](../../aspose.cells.charts/sparklinegroup/lastpointcolor/) { get; set; } | Ottiene e imposta il colore dell'ultimo punto dati nel gruppo di sparkline. |
| [LineWeight](../../aspose.cells.charts/sparklinegroup/lineweight/) { get; set; } | Ottiene e imposta lo spessore della linea in ogni sparkline lineare nel gruppo di sparkline, nell'unità di punti. |
| [LowPointColor](../../aspose.cells.charts/sparklinegroup/lowpointcolor/) { get; set; } | Ottiene e imposta il colore dei punti più bassi dei dati nel gruppo di sparkline. |
| [MarkersColor](../../aspose.cells.charts/sparklinegroup/markerscolor/) { get; set; } | Ottiene e imposta il colore dei punti in ogni sparkline lineare nel gruppo di sparkline. |
| [NegativePointsColor](../../aspose.cells.charts/sparklinegroup/negativepointscolor/) { get; set; } | Ottiene e imposta il colore dei valori negativi nel gruppo di sparkline. |
| [PlotEmptyCellsType](../../aspose.cells.charts/sparklinegroup/plotemptycellstype/) { get; set; } | Indica come tracciare le celle vuote. |
| [PlotRightToLeft](../../aspose.cells.charts/sparklinegroup/plotrighttoleft/) { get; set; } | Indica se i dati del grafico sono da destra a sinistra. |
| [PresetStyle](../../aspose.cells.charts/sparklinegroup/presetstyle/) { get; set; } | Ottiene e imposta il tipo di stile predefinito del gruppo di sparkline. |
| [SeriesColor](../../aspose.cells.charts/sparklinegroup/seriescolor/) { get; set; } | Ottiene e imposta il colore delle sparkline nel gruppo di sparkline. |
| [ShowFirstPoint](../../aspose.cells.charts/sparklinegroup/showfirstpoint/) { get; set; } | Indica se evidenziare il primo punto dati nel gruppo di sparkline. |
| [ShowHighPoint](../../aspose.cells.charts/sparklinegroup/showhighpoint/) { get; set; } | Indica se evidenziare i punti più alti dei dati nel gruppo di sparkline. |
| [ShowHorizontalAxis](../../aspose.cells.charts/sparklinegroup/showhorizontalaxis/) { get; set; } | Indica se mostrare l'asse orizzontale della sparkline. L'asse orizzontale appare se la sparkline ha dati che attraversano l'asse zero. |
| [ShowLastPoint](../../aspose.cells.charts/sparklinegroup/showlastpoint/) { get; set; } | Indica se evidenziare l'ultimo punto dati nel gruppo di sparkline. |
| [ShowLowPoint](../../aspose.cells.charts/sparklinegroup/showlowpoint/) { get; set; } | Indica se evidenziare i punti più bassi dei dati nel gruppo di sparkline. |
| [ShowMarkers](../../aspose.cells.charts/sparklinegroup/showmarkers/) { get; set; } | Indica se evidenziare ogni punto in ogni sparkline a linea nel gruppo di sparkline. |
| [ShowNegativePoints](../../aspose.cells.charts/sparklinegroup/shownegativepoints/) { get; set; } | Indica se evidenziare i valori negativi nel gruppo di sparkline con un colore o un marcatore diverso. |
| [SparklineCollection](../../aspose.cells.charts/sparklinegroup/sparklinecollection/) { get; } | (**Obsolete.**) Ottiene la collezione di oggetti [`Sparkline`](../sparkline/). |
| [Sparklines](../../aspose.cells.charts/sparklinegroup/sparklines/) { get; } | Ottiene la collezione di oggetti [`Sparkline`](../sparkline/). |
| [Type](../../aspose.cells.charts/sparklinegroup/type/) { get; set; } | Indica il tipo di sparkline del gruppo di sparkline. |
| [VerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvalue/) { get; set; } | Ottiene e imposta il valore massimo personalizzato per l'asse verticale. |
| [VerticalAxisMaxValueType](../../aspose.cells.charts/sparklinegroup/verticalaxismaxvaluetype/) { get; set; } | Rappresenta il tipo di valore massimo dell'asse verticale. |
| [VerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/verticalaxisminvalue/) { get; set; } | Ottiene e imposta il valore minimo personalizzato per l'asse verticale. |
| [VerticalAxisMinValueType](../../aspose.cells.charts/sparklinegroup/verticalaxisminvaluetype/) { get; set; } | Rappresenta il tipo di valore minimo dell'asse verticale. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ResetRanges](../../aspose.cells.charts/sparklinegroup/resetranges/)(string, bool, CellArea) | Reimposta l'intervallo di dati e l'intervallo di posizione del gruppo di sparkline. Questo metodo cancellerà gli elementi sparkline originali nel gruppo e creerà nuovi elementi sparkline per i nuovi intervalli. |
| [SetVerticalAxisMaxValue](../../aspose.cells.charts/sparklinegroup/setverticalaxismaxvalue/)(SparklineAxisMinMaxType, double) | Imposta il valore massimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |
| [SetVerticalAxisMinValue](../../aspose.cells.charts/sparklinegroup/setverticalaxisminvalue/)(SparklineAxisMinMaxType, double) | Imposta il valore minimo personalizzato per l'asse verticale dello sparkline con il tipo di valore dell'asse specificato. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupDemo
    {
        public static void SparklineGroupExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati al worksheet
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definisci il CellArea per lo sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Aggiungi un gruppo di sparkline al foglio di lavoro
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Aggiungi sparkline al gruppo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Crea CellsColor per il colore della serie
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Orange;
            group.SeriesColor = seriesColor;

            // Imposta i punti alti colorati di verde e i punti bassi colorati di rosso
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = Color.Green;
            group.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = Color.Red;
            group.LowPointColor = lowPointColor;

            // Imposta lo spessore della linea
            group.LineWeight = 1.0;

            // Imposta proprietà aggiuntive
            group.PresetStyle = SparklinePresetStyleType.Style1;
            group.Type = SparklineType.Line;
            group.PlotEmptyCellsType = PlotEmptyCellsType.Zero;
            group.DisplayHidden = true;
            group.ShowNegativePoints = true;
            CellsColor negativePointsColor = workbook.CreateCellsColor();
            negativePointsColor.Color = Color.Blue;
            group.NegativePointsColor = negativePointsColor;

            group.ShowFirstPoint = true;
            CellsColor firstPointColor = workbook.CreateCellsColor();
            firstPointColor.Color = Color.Purple;
            group.FirstPointColor = firstPointColor;

            group.ShowLastPoint = true;
            CellsColor lastPointColor = workbook.CreateCellsColor();
            lastPointColor.Color = Color.Yellow;
            group.LastPointColor = lastPointColor;

            group.ShowMarkers = true;
            CellsColor markersColor = workbook.CreateCellsColor();
            markersColor.Color = Color.Black;
            group.MarkersColor = markersColor;

            group.PlotRightToLeft = false;
            CellsColor horizontalAxisColor = workbook.CreateCellsColor();
            horizontalAxisColor.Color = Color.Gray;
            group.HorizontalAxisColor = horizontalAxisColor;

            group.ShowHorizontalAxis = true;
            group.HorizontalAxisDateRange = "A1:D1";
            group.VerticalAxisMaxValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMaxValue = 10.0;
            group.VerticalAxisMinValueType = SparklineAxisMinMaxType.Group;
            group.VerticalAxisMinValue = 0.0;

            // Salva la cartella di lavoro
            workbook.Save("SparklineGroupExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


