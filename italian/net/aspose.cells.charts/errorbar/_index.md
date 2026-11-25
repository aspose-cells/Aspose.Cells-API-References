---
title: "Classe ErrorBar"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ErrorBar class. Rappresenta la barra di errore della serie di dati"
type: docs
url: /it/net/aspose.cells.charts/errorbar/
---
## ErrorBar class

Rappresenta la barra di errore della serie di dati.

```csharp
public class ErrorBar : Line
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Amount](../../aspose.cells.charts/errorbar/amount/) { get; set; } | Rappresenta la quantità della barra di errore. |
| [BeginArrowLength](../../aspose.cells.drawing/line/beginarrowlength/) { get; set; } | Specifica la lunghezza della punta della freccia per l'inizio di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginArrowWidth](../../aspose.cells.drawing/line/beginarrowwidth/) { get; set; } | Specifica la larghezza della punta della freccia per l'inizio di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [BeginType](../../aspose.cells.drawing/line/begintype/) { get; set; } | Specifica una punta di freccia per l'inizio di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [CapType](../../aspose.cells.drawing/line/captype/) { get; set; } | Specifica le estremità finali.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [Color](../../aspose.cells.drawing/line/color/) { get; set; } | Rappresenta il colore della linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [CompoundType](../../aspose.cells.drawing/line/compoundtype/) { get; set; } | Specifica il tipo di linea composta (Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [DashType](../../aspose.cells.drawing/line/dashtype/) { get; set; } | Specifica il tipo di linea tratteggiata (Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [DisplayType](../../aspose.cells.charts/errorbar/displaytype/) { get; set; } | Rappresenta il tipo di visualizzazione della barra di errore. |
| [EndArrowLength](../../aspose.cells.drawing/line/endarrowlength/) { get; set; } | Specifica la lunghezza della punta della freccia per la fine di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [EndArrowWidth](../../aspose.cells.drawing/line/endarrowwidth/) { get; set; } | Specifica la larghezza della punta della freccia per la fine di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [EndType](../../aspose.cells.drawing/line/endtype/) { get; set; } | Specifica una punta di freccia per la fine di una linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [FormattingType](../../aspose.cells.drawing/line/formattingtype/) { get; set; } | Ottiene o imposta il tipo di formato.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [GradientFill](../../aspose.cells.drawing/line/gradientfill/) { get; } | Rappresenta il riempimento gradiente.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAuto](../../aspose.cells.drawing/line/isauto/) { get; set; } | Indica se questo stile di linea è assegnato automaticamente.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [IsAutomaticColor](../../aspose.cells.drawing/line/isautomaticcolor/) { get; } | Indica se il colore della linea è assegnato automaticamente.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [IsVisible](../../aspose.cells.drawing/line/isvisible/) { get; set; } | Rappresenta se la linea è visibile.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [JoinType](../../aspose.cells.drawing/line/jointype/) { get; set; } | Specifica le estremità di giunzione.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [MinusValue](../../aspose.cells.charts/errorbar/minusvalue/) { get; set; } | Rappresenta la quantità di errore negativa quando il tipo di barra di errore è Personalizzato. |
| [PlusValue](../../aspose.cells.charts/errorbar/plusvalue/) { get; set; } | Rappresenta la quantità di errore positiva quando il tipo di barra di errore è Personalizzato. |
| [ShowMarkerTTop](../../aspose.cells.charts/errorbar/showmarkerttop/) { get; set; } | Indica se formattare le barre di errore con una T superiore. |
| [Style](../../aspose.cells.drawing/line/style/) { get; set; } | Rappresenta lo stile della linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [ThemeColor](../../aspose.cells.drawing/line/themecolor/) { get; set; } | Ottiene e imposta il colore del tema.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [Transparency](../../aspose.cells.drawing/line/transparency/) { get; set; } | Restituisce o imposta il grado di trasparenza della linea come valore da 0.0 (opaco) a 1.0 (trasparente).(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [Type](../../aspose.cells.charts/errorbar/type/) { get; set; } | Rappresenta il tipo di quantità della barra di errore. |
| [Weight](../../aspose.cells.drawing/line/weight/) { get; set; } | Ottiene o imposta il [`WeightType`](../../aspose.cells.drawing/weighttype/) della linea.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPt](../../aspose.cells.drawing/line/weightpt/) { get; set; } | Ottiene o imposta il peso della linea in unità di punti.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |
| [WeightPx](../../aspose.cells.drawing/line/weightpx/) { get; set; } | Ottiene o imposta il peso della linea in unità di pixel.(Ereditato da [`Line`](../../aspose.cells.drawing/line/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDemo
    {
        public static void ErrorBarExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Aggiungi dati di esempio alle celle
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);
            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];

            // Aggiungi NSeries (origine dati del grafico) al grafico
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configura le barre di errore per ogni serie nel grafico
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;

                // Proprietà aggiuntive per la dimostrazione
                series.YErrorBar.ShowMarkerTTop = true;
                series.YErrorBar.PlusValue = "=Sheet1!A1";
                series.YErrorBar.MinusValue = "=Sheet1!A2";
                series.YErrorBar.CompoundType = Aspose.Cells.Drawing.MsoLineStyle.ThickThin;
                series.YErrorBar.DashType = Aspose.Cells.Drawing.MsoLineDashStyle.DashDot;
                series.YErrorBar.CapType = Aspose.Cells.Drawing.LineCapType.Round;
                series.YErrorBar.JoinType = Aspose.Cells.Drawing.LineJoinType.Bevel;
                series.YErrorBar.BeginType = Aspose.Cells.Drawing.MsoArrowheadStyle.Arrow;
                series.YErrorBar.EndType = Aspose.Cells.Drawing.MsoArrowheadStyle.ArrowDiamond;
                series.YErrorBar.BeginArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Short;
                series.YErrorBar.EndArrowLength = Aspose.Cells.Drawing.MsoArrowheadLength.Long;
                series.YErrorBar.BeginArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Narrow;
                series.YErrorBar.EndArrowWidth = Aspose.Cells.Drawing.MsoArrowheadWidth.Wide;
                series.YErrorBar.ThemeColor = new Aspose.Cells.ThemeColor(Aspose.Cells.ThemeColorType.Accent1, 0.5);
                series.YErrorBar.Color = System.Drawing.Color.Red;
                series.YErrorBar.Transparency = 0.5;
                series.YErrorBar.Style = Aspose.Cells.Drawing.LineType.DashDotDot;
                series.YErrorBar.Weight = Aspose.Cells.Drawing.WeightType.WideLine;
                series.YErrorBar.WeightPt = 2.0;
                series.YErrorBar.WeightPx = 3.0;
                series.YErrorBar.FormattingType = ChartLineFormattingType.Gradient;
                series.YErrorBar.IsVisible = true;
                series.YErrorBar.IsAuto = false;
            }

            // Salva la cartella di lavoro
            workbook.Save("ErrorBarExample.xlsx");
            workbook.Save("ErrorBarExample.pdf");
        }
    }
}
```

### Vedi anche

* class [Line](../../aspose.cells.drawing/line/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


