---
title: "Klasse Walls"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.Walls‑Klasse. Kapselt das Objekt, das die Wände eines 3D‑Diagramms darstellt."
type: docs
url: /de/net/aspose.cells.charts/walls/
---
## Walls class

Kapselt das Objekt, das die Wände eines 3‑D-Diagramms darstellt.

```csharp
public class Walls : Floor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Liest oder setzt die Hintergrundfarbe des [`Area`](../../aspose.cells.drawing/area/). (Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Liest oder setzt die Begrenzung [`Line`](../../aspose.cells.drawing/line/).(Vererbt von [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Liest die x‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Liest die y‑Koordinate der linken unteren Ecke des Wandzentrums in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Liest die Tiefe von vorne nach hinten in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Liest die Tiefe von vorne nach hinten in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Stellt ein [`FillFormat`](../../aspose.cells.drawing/area/fillformat/) Objekt dar, das Füllformatierungs‑Eigenschaften für das angegebene Diagramm oder die Form enthält.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Liest oder setzt die Vordergrundfarbe.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Stellt die Formatierung des Bereichs dar.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Liest die Höhe von oben nach unten in Einheiten von 1/4000 der Diagrammhöhe nach Aufruf der Methode Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Liest die Höhe von oben nach unten in Pixeln nach Aufruf der Methode Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Wenn die Eigenschaft true ist und der Wert des Diagrammpunkts eine negative Zahl ist, werden die Vordergrund‑ und Hintergrundfarbe vertauscht.(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Liefert oder setzt den Transparenzgrad des Bereichs als Wert von 0.0 (undurchsichtig) bis 1.0 (klar).(Vererbt von [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Liest die Breite von links nach rechts in Einheiten von 1/4000 der Diagrammbreite nach Aufruf der Methode Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Liest die Breite von links nach rechts in Pixeln nach Aufruf der Methode Chart.Calculate(). |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Liest die Anzahl der Würfelpunkte nach Aufruf der Methode Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Liest die x‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht. |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Liest die y‑Koordinate des Scheitelpunkts des Wandwürfels nach Aufruf der Methode Chart.Calculate(). Die Anzahl der Scheitelpunkte des Wandwürfels beträgt acht. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Fügen Sie ein 3D‑Diagramm zum Arbeitsblatt hinzu.
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Berechnen Sie das Diagramm, um seine Eigenschaften zu aktualisieren.
            chart.Calculate();

            // Zugriff auf die Wände des 3D‑Diagramms.
            Walls walls = chart.Walls;

            // Eigenschaften der Wände festlegen.
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Zugriff auf die Begrenzung der Wände und deren Eigenschaften festlegen.
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Einige Eigenschaften der Wände ausgeben.
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

            // Speichere die Arbeitsmappe
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


