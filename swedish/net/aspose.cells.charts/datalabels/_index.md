---
title: "Klassen DataLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.DataLabels-klass. Inkapslar en samling av alla DataLabel-objekt för den angivna serien"
type: docs
url: /sv/net/aspose.cells.charts/datalabels/
---
## DataLabels class

Inkapslar en samling av alla DataLabel-objekt för den angivna serien.

```csharp
public class DataLabels : ChartTextFrame
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [Area](../../aspose.cells.charts/datalabels/area/) { get; } | Hämtar [`area`](./area/). |
| virtual [AutoScaleFont](../../aspose.cells.charts/chartframe/autoscalefont/) { get; set; } | Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Obsolete.**) Hämtar och anger visningsläget för bakgrunden. Denna egenskap är endast giltig i Excel 2003 eller tidigare versioner.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/datalabels/backgroundmode/) { get; set; } | Hämtar och anger visningsläget för bakgrunden |
| override [Border](../../aspose.cells.charts/datalabels/border/) { get; } | Hämtar [`border`](../../aspose.cells.drawing/line/). |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Obsolete.**) Representerar höjden för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Representerar höjden för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Obsolete.**) Representerar bredden för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Representerar bredden för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Obsolete.**) Representerar x för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Representerar x för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Obsolete.**) Representerar y för standardpositionen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Representerar y för standardpositionen i enheter av en bråkdel av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| override [DirectionType](../../aspose.cells.charts/datalabels/directiontype/) { get; set; } | Hämtar och anger textens riktning. |
| override [Font](../../aspose.cells.charts/datalabels/font/) { get; } | Hämtar teckensnittet för DataLabels; |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Obsolete.**) Hämtar eller anger höjden på ramen i enheter av 1/4000 av diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Hämtar eller anger höjden på ramen i pixelenheter.(Ärvd från [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Hämtar eller anger höjden på ramen i enheter av förhållandet till diagramområdet.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Anger om diagramtexten roteras automatiskt.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Anger om diagramramen har automatisk storlek.(Ärvd från [`ChartFrame`](../chartframe/).) |
| override [IsAutoText](../../aspose.cells.charts/datalabels/isautotext/) { get; set; } | Indikerar att texten är automatiskt genererad. |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Anger om standardpositionen (DefaultX, DefaultY, DefaultWidth och DefaultHeight) är angiven.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Anger om denna datamärkning är raderad.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Anger om storleken på plotområdet inkluderar stapelmärken och axelrubriker. Falskt betyder att storleken ska bestämma storleken på plotområdet, stapelmärkena och axelrubrikerna.(Ärvd från [`ChartFrame`](../chartframe/).) |
| [IsNeverOverlap](../../aspose.cells.charts/datalabels/isneveroverlap/) { get; set; } | Indikerar om Datalabels aldrig överlappar när en pajdiagram konverteras till bild. Obs: den här egenskapen är endast meningsfull när en pajdiagram konverteras till bild. |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Hämtar eller anger huruvida en form ska automatiskt anpassas för att helt innehålla den text som beskrivs i den. Automatisk anpassning är när text inom en form skalas för att innehålla all text inuti.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| override [IsTextWrapped](../../aspose.cells.charts/datalabels/istextwrapped/) { get; set; } | Hämtar eller anger ett värde som indikerar om texten är radbruten. |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Hämtar och anger en referens till kalkylbladet.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [Number](../../aspose.cells.charts/datalabels/number/) { get; set; } | Hämtar och anger det inbyggda talformatet. |
| [NumberFormat](../../aspose.cells.charts/datalabels/numberformat/) { get; set; } | Representerar formatsträngen för DataLabels-objektet. |
| [NumberFormatLinked](../../aspose.cells.charts/datalabels/numberformatlinked/) { get; set; } | Sant om talformatet är länkat till cellerna (så att talformatet ändras i etiketterna när det ändras i cellerna). |
| [Position](../../aspose.cells.charts/datalabels/position/) { get; set; } | Representerar positionen för datamärket. |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Representerar läsriktning för text.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Representerar textens rotationsvinkel.(Inherited from [`ChartTextFrame`](../charttextframe/).) |
| [SeparatorType](../../aspose.cells.charts/datalabels/separatortype/) { get; set; } | Hämtar eller anger separatorns typ som används för datamärken i ett diagram. |
| [SeparatorValue](../../aspose.cells.charts/datalabels/separatorvalue/) { get; set; } | Hämtar eller anger separatorns värde som används för datamärken i ett diagram. |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Sant om ramen har en skugga.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Hämtar [`ShapeProperties`](../chartframe/shapeproperties/)‑objektet.(Inherited from [`ChartFrame`](../chartframe/).) |
| [ShapeType](../../aspose.cells.charts/datalabels/shapetype/) { get; set; } | Hämtar eller anger formtypen för datamärket. |
| [ShowBubbleSize](../../aspose.cells.charts/datalabels/showbubblesize/) { get; set; } | Representerar ett specificerat diagrammets visningsbeteende för datamärkets procentvärde. Sant visar procentvärdet. Falskt döljer procentvärdet. |
| [ShowCategoryName](../../aspose.cells.charts/datalabels/showcategoryname/) { get; set; } | Representerar ett specificerat diagrammets visningsbeteende för datamärkets kategorinamn. Sant för att visa kategorinamnet för datamärken i ett diagram. Falskt för att dölja. |
| [ShowCellRange](../../aspose.cells.charts/datalabels/showcellrange/) { get; set; } | Indikerar om cellområdet ska visas som datamärken. |
| [ShowLegendKey](../../aspose.cells.charts/datalabels/showlegendkey/) { get; set; } | Representerar ett specificerat diagrammets visningsbeteende för datamärkets legendnyckel. Sant om legendnyckeln för datamärket är synlig. |
| [ShowPercentage](../../aspose.cells.charts/datalabels/showpercentage/) { get; set; } | Representerar ett specificerat diagrammets dataetiketts procentsatsvisningsbeteende. True visar procentsatsen. False för att dölja. |
| [ShowSeriesName](../../aspose.cells.charts/datalabels/showseriesname/) { get; set; } | Anger om seriens namn visas på dataetiketterna i ett diagram. True för att visa seriens namn. False för att dölja. |
| [ShowValue](../../aspose.cells.charts/datalabels/showvalue/) { get; set; } | Representerar ett specificerat diagrammets dataetiketts värdevisningsbeteende. True visar värdena. False för att dölja. |
| override [Text](../../aspose.cells.charts/datalabels/text/) { get; set; } | Hämtar eller anger texten för dataetiketten. |
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
| [ApplyFont](../../aspose.cells.charts/datalabels/applyfont/)() | Applicera teckensnittet för dataetiketterna på alla underordnade noder. |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Returnerar ett Characters-objekt som representerar ett teckenintervall inom texten.(Ärvd från [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Ställ in positionen för ramen till automatisk.(Ärvd från [`ChartFrame`](../chartframe/).) |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DataLabelsDemo
    {
        public static void DataLabelsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lägg till serier i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till DataLabels för den första serien
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Ställ in egenskaper för DataLabels
            dataLabels.Position = LabelPositionType.InsideBase;
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.ShowPercentage = false;
            dataLabels.ShowLegendKey = false;
            dataLabels.IsAutoText = true;
            dataLabels.DirectionType = ChartTextDirectionType.Horizontal;
            dataLabels.Text = "Custom Text";
            dataLabels.IsTextWrapped = true;
            dataLabels.BackgroundMode = BackgroundMode.Transparent;
            dataLabels.ShowCellRange = false;
            dataLabels.ShowBubbleSize = false;
            dataLabels.ShowSeriesName = false;
            dataLabels.NumberFormat = "0.00";
            dataLabels.Number = 0;
            dataLabels.NumberFormatLinked = false;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;
            dataLabels.SeparatorValue = ", ";
            dataLabels.IsNeverOverlap = true;
            dataLabels.IsDeleted = false;
            dataLabels.TextHorizontalAlignment = TextAlignmentType.Center;
            dataLabels.TextVerticalAlignment = TextAlignmentType.Center;
            dataLabels.RotationAngle = 0;
            dataLabels.LinkedSource = "";
            dataLabels.TextDirection = TextDirectionType.LeftToRight;
            dataLabels.ReadingOrder = TextDirectionType.LeftToRight;
            dataLabels.IsResizeShapeToFitText = true;
            dataLabels.IsInnerMode = false;
            dataLabels.AutoScaleFont = true;
            dataLabels.Background = BackgroundMode.Transparent;
            dataLabels.IsAutomaticSize = true;
            dataLabels.X = 0;
            dataLabels.Y = 0;
            dataLabels.Height = 100;
            dataLabels.Width = 100;
            dataLabels.Shadow = false;

            // Spara arbetsboken
            workbook.Save("DataLabelsExample.xlsx");
            workbook.Save("DataLabelsExample.pdf");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


