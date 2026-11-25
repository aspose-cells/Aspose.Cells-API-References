---
title: "Classe Walls"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.Walls. Incapsula l'oggetto che rappresenta le pareti di un grafico 3D"
type: docs
url: /it/net/aspose.cells.charts/walls/
---
## Walls class

Incapsula l'oggetto che rappresenta le pareti di un grafico 3-D.

```csharp
public class Walls : Floor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Ottiene o imposta il colore di sfondo del [`Area`](../../aspose.cells.drawing/area/). (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Ottiene o imposta il bordo [`Line`](../../aspose.cells.drawing/line/). (Ereditato da [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Ottiene la coordinata x dell'angolo sinistro-inferiore del centro della parete in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Ottiene la coordinata x dell'angolo inferiore-sinistro del centro della parete in unità di pixel dopo la chiamata al metodo Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Ottiene la coordinata y dell'angolo sinistro-inferiore del centro della parete in unità di 1/4000 dell'altezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Ottiene la coordinata y dell'angolo sinistro-inferiore del centro della parete in unità di pixel dopo le chiamate al metodo Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Ottiene la profondità da davanti a dietro in unità di 1/4000 della larghezza del grafico dopo la chiamata al metodo Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Ottiene la profondità da fronte a retro in unità di pixel dopo le chiamate al metodo Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Rappresenta un oggetto [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Ottiene o imposta il colore di primo piano. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Rappresenta la formattazione dell'area. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Ottiene l'altezza dall'alto verso il basso in unità di 1/4000 dell'altezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Ottiene l'altezza dall'alto verso il basso in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Se la proprietà è true e il valore del punto del grafico è un numero negativo, il colore di primo piano e il colore di sfondo verranno scambiati. (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 (opaco) a 1.0 (chiaro). (Ereditato da [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Ottiene la larghezza da sinistra a destra in unità di 1/4000 della larghezza del grafico dopo le chiamate al metodo Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Ottiene la larghezza da sinistra a destra in unità di pixel dopo aver chiamato il metodo Chart.Calculate(). |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Ottiene il numero di punti del cubo dopo le chiamate al metodo Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Ottiene la coordinata x del punto apice del cubo delle pareti dopo aver chiamato il metodo Chart.Calculate(). Il numero di punti apice del cubo delle pareti è otto. |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Ottiene la coordinata y del punto apice del cubo delle pareti dopo le chiamate al metodo Chart.Calculate(). Il numero di punti apice del cubo delle pareti è otto. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class WallsDemo
    {
        public static void WallsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico 3D al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcola il grafico per aggiornare le sue proprietà
            chart.Calculate();

            // Accedi alle pareti del grafico 3D
            Walls walls = chart.Walls;

            // Imposta le proprietà delle pareti
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Accedi al bordo delle pareti e imposta le sue proprietà
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Stampa alcune proprietà delle pareti
            Console.WriteLine("CenterX: " + walls.CenterX);
            Console.WriteLine("CenterY: " + walls.CenterY);
            Console.WriteLine("Width: " + walls.Width);
            Console.WriteLine("Depth: " + walls.Depth);
            Console.WriteLine("Height: " + walls.Height);
            Console.WriteLine("CenterXPx: " + walls.CenterXPx);
            Console.WriteLine("CenterYPx: " + walls.CenterYPx);
            Console.WriteLine("WidthPx: " + walls.WidthPx);
            Console.WriteLine("DepthPx: " + walls.DepthPx);
            Console.WriteLine("HeightPx: " + walls.HeightPx);

            // Salva la cartella di lavoro
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


