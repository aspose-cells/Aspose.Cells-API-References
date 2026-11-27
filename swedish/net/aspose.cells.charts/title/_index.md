---
title: "Klassrubrik"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.Title class. Inkapslar objektet som representerar titeln på diagrammet eller axeln"
type: docs
url: /sv/net/aspose.cells.charts/title/
---
## Title class

Inkapslar objektet som representerar titeln på diagrammet eller axeln.

```csharp
public class Title : ChartTextFrame
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Hämtar [`area`](../chartframe/area/).(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Obsolete.**) Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Hämtar [`border`](../../aspose.cells.drawing/line/).(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Representerar höjden för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Representerar bredden för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Representerar x för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Representerar x för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Representerar y för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Representerar y för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | Hämtar och anger textens riktning.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| virtual [Font](../../aspose.cells.charts/chartframe/font/) { get; } | Hämtar ett [`Font`](../chartframe/font/) objekt för det angivna ChartFrame-objektet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Hämtar eller anger höjden på ramen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Hämtar eller anger höjden på ramen i pixelenheter.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Hämtar eller anger höjden på ramen i enheter av förhållandet till diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Anger om diagramtexten roteras automatiskt.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Anger om diagramramen har automatisk storlek.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | Anger att texten är automatiskt genererad.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Anger om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Anger om denna datamärkning är raderad.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Anger om storleken på plotområdet inkluderar stapelmärken och axelrubriker. Falskt betyder att storleken ska bestämma storleken på plotområdet, stapelmärkena och axelrubrikerna.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Hämtar eller anger huruvida en form ska automatiskt anpassas för att helt innehålla den text som beskrivs i den. Automatisk anpassning är när text inom en form skalas för att innehålla all text inuti.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Hämtar eller anger ett värde som indikerar om texten är radbruten.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [IsVisible](../../aspose.cells.charts/title/isvisible/) { get; set; } | Representerar huruvida titeln är synlig. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Hämtar och anger en referens till kalkylbladet.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [OverLay](../../aspose.cells.charts/title/overlay/) { get; set; } | Representerar en överlagrad centrerad titel på ett diagram utan att ändra diagrammets storlek. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Representerar läsriktning för text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Representerar textens rotationsvinkel.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Sant om ramen har en skugga.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Hämtar [`ShapeProperties`](../chartframe/shapeproperties/)‑objektet.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/title/text/) { get; set; } | Hämtar eller anger texten för displayenhetsetiketten. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Representerar läsriktning för text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Hämtar ett [`Font`](../chartframe/font/)‑objekt för det angivna ChartFrame‑objektet.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Hämtar och anger den horisontella justeringen av texten.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Hämtar och anger alternativen för texten.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Hämtar eller anger den vertikala justeringen av texten.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Hämtar eller anger ramens bredd i enheter av 1/4000 av diagramområdet.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Hämtar eller anger ramens bredd i enheter av pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Hämtar eller anger ramens bredd i enheter av förhållandet till diagramområdet.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [X](../../aspose.cells.charts/title/x/) { get; set; } | (**Obsolete.**) Hämtar eller anger X‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [XRatioToChart](../../aspose.cells.charts/title/xratiotochart/) { get; set; } | Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. X i pixlar = XRatioToChart * Chart.ChartObject.Width; |
| override [Y](../../aspose.cells.charts/title/y/) { get; set; } | (**Obsolete.**) Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av pixlar.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [YRatioToChart](../../aspose.cells.charts/title/yratiotochart/) { get; set; } | Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av bråkdel av diagramområdet. Y i pixlar = YRatioToChart * Chart.ChartObject.Width; |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Characters](../../aspose.cells.charts/title/characters/#characters_1)() | Hämtar rik textformatering för den här titeln. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Returnerar ett Characters-objekt som representerar ett teckenintervall inom texten.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Ställ in positionen för ramen till automatisk.(Ärvd från [`ChartFrame`](../chartframe/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TitleDemo
    {
        public static void TitleExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata i kalkylbladet
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];

            // Ange datakällan för diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ange diagrammets titel
            chart.Title.Text = "Income Analysis";
            chart.Title.Font.Color = Color.Blue;
            chart.Title.IsVisible = true;
            chart.Title.X = 100;
            chart.Title.Y = 50;
            chart.Title.OverLay = false;
            chart.Title.IsAutoText = false;
            chart.Title.IsDeleted = false;
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Center;
            chart.Title.RotationAngle = 0;
            chart.Title.LinkedSource = null;
            chart.Title.TextDirection = TextDirectionType.LeftToRight;
            chart.Title.ReadingOrder = TextDirectionType.LeftToRight;
            chart.Title.DirectionType = ChartTextDirectionType.Horizontal;
            chart.Title.IsTextWrapped = true;
            chart.Title.IsResizeShapeToFitText = true;
            chart.Title.IsInnerMode = false;
            chart.Title.AutoScaleFont = true;
            chart.Title.BackgroundMode = BackgroundMode.Transparent;
            chart.Title.IsAutomaticSize = true;
            chart.Title.Height = 100;
            chart.Title.Width = 200;
            chart.Title.Shadow = false;

            // Spara arbetsboken
            workbook.Save("TitleExample.xlsx");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


