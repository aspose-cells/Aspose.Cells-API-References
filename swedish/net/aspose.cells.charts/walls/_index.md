---
title: "Klass Walls"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Walls-klass. Inkapslar objektet som representerar väggarna i ett 3D-diagram"
type: docs
url: /sv/net/aspose.cells.charts/walls/
---
## Walls class

Inkapslar objektet som representerar väggarna i ett 3‑D‑diagram.

```csharp
public class Walls : Floor
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Hämtar eller anger bakgrundsfärgen för [`Area`](../../aspose.cells.drawing/area/).(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Border](../../aspose.cells.charts/floor/border/) { get; set; } | Hämtar eller anger kanten [`Line`](../../aspose.cells.drawing/line/).(Arv från [`Floor`](../floor/).) |
| [CenterX](../../aspose.cells.charts/walls/centerx/) { get; } | Hämtar x-koordinaten för vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [CenterXPx](../../aspose.cells.charts/walls/centerxpx/) { get; } | Hämtar x-koordinaten för nedre‑vänstra hörnet av väggens centrum i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [CenterY](../../aspose.cells.charts/walls/centery/) { get; } | Hämtar y-koordinaten för vänster‑nedre hörnet av väggens centrum i enheter av 1/4000 av diagrammets höjd efter att ha anropat metoden Chart.Calculate(). |
| [CenterYPx](../../aspose.cells.charts/walls/centerypx/) { get; } | Hämtar y-koordinaten för vänster‑nedre hörnet av väggens centrum i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [Depth](../../aspose.cells.charts/walls/depth/) { get; } | Hämtar djupet fram till bak i enheter av 1/4000 av diagrammets bredd efter att ha anropat metoden Chart.Calculate(). |
| [DepthPx](../../aspose.cells.charts/walls/depthpx/) { get; } | Hämtar djupet fram till bak i pixelenheter efter anrop av metoden Chart.Calculate(). |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Representerar ett [`FillFormat`](../../aspose.cells.drawing/area/fillformat/)‑objekt som innehåller fyllningsformaterings‑egenskaper för det angivna diagrammet eller formen.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Hämtar eller anger förgrundsfärgen.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Representerar formateringen av området.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Height](../../aspose.cells.charts/walls/height/) { get; } | Hämtar höjden från topp till botten i enheter av 1/4000 av diagrammets höjd efter anrop av metoden Chart.Calculate(). |
| [HeightPx](../../aspose.cells.charts/walls/heightpx/) { get; } | Hämtar höjden från topp till botten i pixelenheter efter att ha anropat metoden Chart.Calculate(). |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas ut.(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Returnerar eller anger graden av transparens för området som ett värde från 0.0 (opak) genom 1.0 (klar).(Ärvd från [`Area`](../../aspose.cells.drawing/area/).) |
| [Width](../../aspose.cells.charts/walls/width/) { get; } | Hämtar bredden från vänster till höger i enheter av 1/4000 av diagrammets bredd efter anrop av metoden Chart.Calculate(). |
| [WidthPx](../../aspose.cells.charts/walls/widthpx/) { get; } | Hämtar bredden från vänster till höger i pixelenheter efter att ha anropat metoden Chart.Calculate(). |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetCubePointCount](../../aspose.cells.charts/walls/getcubepointcount/)() | Hämtar antalet kubpunkter efter anrop av metoden Chart.Calculate(). |
| [GetCubePointXPx](../../aspose.cells.charts/walls/getcubepointxpx/)(int) | Hämtar x-koordinaten för apex-punkten i väggkuben efter att ha anropat metoden Chart.Calculate(). Antalet apex-punkter i väggkuben är åtta |
| [GetCubePointYPx](../../aspose.cells.charts/walls/getcubepointypx/)(int) | Hämtar y-koordinaten för apex-punkten i väggkuben efter anrop av metoden Chart.Calculate(). Antalet apex-punkter i väggkuben är åtta. |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett 3D-diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Beräkna diagrammet för att uppdatera dess egenskaper
            chart.Calculate();

            // Kom åt väggarna i 3D-diagrammet
            Walls walls = chart.Walls;

            // Ställ in egenskaper för väggarna
            walls.BackgroundColor = Color.LightBlue;
            walls.ForegroundColor = Color.DarkBlue;
            walls.Formatting = FormattingType.Custom;
            walls.InvertIfNegative = true;
            walls.Transparency = 0.5;

            // Få åtkomst till väggarnas kant och ställ in dess egenskaper
            Line border = walls.Border;
            border.Color = Color.Red;
            border.Style = LineType.Solid;

            // Skriv ut vissa egenskaper för väggarna
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

            // Spara arbetsboken
            workbook.Save("WallsExample.xlsx");
        }
    }
}
```

### Se även

* class [Floor](../floor/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


