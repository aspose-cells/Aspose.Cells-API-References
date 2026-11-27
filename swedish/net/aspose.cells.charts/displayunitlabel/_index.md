---
title: "Klass DisplayUnitLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.DisplayUnitLabel-klass. Representerar displayenhetsetiketten"
type: docs
url: /sv/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Representerar etiketten för visningsenheten.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Hämtar [`area`](../chartframe/area/).(Ärvd från [`ChartFrame`](../chartframe/).) |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant. |
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
| override [Font](../../aspose.cells.charts/displayunitlabel/font/) { get; } | Hämtar ett [`Font`](./font/)‑objekt för det angivna ChartFrame‑objektet. |
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
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Hämtar och anger en referens till kalkylbladet.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Representerar läsriktning för text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Representerar textens rotationsvinkel.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Sant om ramen har en skugga.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Hämtar [`ShapeProperties`](../chartframe/shapeproperties/)‑objektet.(Inherited from [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/displayunitlabel/text/) { get; set; } | Hämtar eller anger texten för displayenhetsetiketten. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Representerar läsriktning för text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Hämtar ett [`Font`](../chartframe/font/)‑objekt för det angivna ChartFrame‑objektet.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Hämtar och anger den horisontella justeringen av texten.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Hämtar och anger alternativen för texten.(Inherited from [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Hämtar eller anger den vertikala justeringen av texten.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Hämtar eller anger ramens bredd i enheter av 1/4000 av diagramområdet.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Hämtar eller anger ramens bredd i enheter av pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Hämtar eller anger ramens bredd i enheter av förhållandet till diagramområdet.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Föråldrad.**) Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i enheter av pixel.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Hämtar eller anger x‑koordinaten för det övre vänstra hörnet i förhållande till diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Föråldrad.**) Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i enheter av pixlar.(Inherited from [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Hämtar eller anger y‑koordinaten för det övre vänstra hörnet i förhållande till diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
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

    public class DisplayUnitLabelDemo
    {
        public static void DisplayUnitLabelExample()
        {
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            // Lägga till ett nytt kalkylblad i Workbook-objektet
            int sheetIndex = workbook.Worksheets.Add();
            // Hämtar referensen till det nyligen tillagda kalkylbladet genom att ange dess bladindex
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Lägger till exempelvärden i celler
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

            // Lägger till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Åtkomst till instansen av det nyligen tillagda diagrammet
            Chart chart = worksheet.Charts[chartIndex];
            // Lägger till NSeries (diagramdatakälla) i diagrammet från cellen "A1" till "B4"
            chart.NSeries.Add("A1:B4", true);
            // Anger datakällan för kategoridata i NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Ställer in displayenheten för värde(Y)-axeln
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Ställer in egenskaper för DisplayUnitLabel
            displayUnitLabel.Text = "100";
            displayUnitLabel.AutoScaleFont = true;
            displayUnitLabel.IsAutoText = false;
            displayUnitLabel.IsDeleted = false;
            displayUnitLabel.TextHorizontalAlignment = TextAlignmentType.Center;
            displayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;
            displayUnitLabel.RotationAngle = 0;
            displayUnitLabel.LinkedSource = "";
            displayUnitLabel.TextDirection = TextDirectionType.LeftToRight;
            displayUnitLabel.ReadingOrder = TextDirectionType.LeftToRight;
            displayUnitLabel.DirectionType = ChartTextDirectionType.Horizontal;
            displayUnitLabel.IsTextWrapped = false;
            displayUnitLabel.IsResizeShapeToFitText = false;
            displayUnitLabel.IsInnerMode = false;
            displayUnitLabel.BackgroundMode = BackgroundMode.Transparent;
            displayUnitLabel.IsAutomaticSize = true;
            displayUnitLabel.X = 0;
            displayUnitLabel.Y = 0;
            displayUnitLabel.Height = 100;
            displayUnitLabel.Width = 100;
            displayUnitLabel.Shadow = false;

            // Sparar Excel-filen
            workbook.Save("DisplayUnitLabelExample.xlsx");
            workbook.Save("DisplayUnitLabelExample.pdf");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


