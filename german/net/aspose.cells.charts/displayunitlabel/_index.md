---
title: "Klasse DisplayUnitLabel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.DisplayUnitLabel Klasse. Stellt das Anzeigeeinheiten‑Label dar"
type: docs
url: /de/net/aspose.cells.charts/displayunitlabel/
---
## DisplayUnitLabel class

Stellt das Anzeigeeinheiten-Label dar.

```csharp
public class DisplayUnitLabel : ChartTextFrame
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| virtual [Area](../../aspose.cells.charts/chartframe/area/) { get; } | Ruft das [`area`](../chartframe/area/).(Geerbt von [`ChartFrame`](../chartframe/).) |
| override [AutoScaleFont](../../aspose.cells.charts/displayunitlabel/autoscalefont/) { get; set; } | True, wenn der Text im Objekt die Schriftgröße ändert, wenn die Objektgröße geändert wird. Der Standardwert ist True. |
| [Background](../../aspose.cells.charts/chartframe/background/) { get; set; } | (**Veraltet.**) Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.(Geerbt von [`ChartFrame`](../chartframe/).) |
| [BackgroundMode](../../aspose.cells.charts/chartframe/backgroundmode/) { get; set; } | (**Veraltet.**) Ruft den Anzeigemodus des Hintergrunds ab und legt ihn fest. Diese Eigenschaft ist nur in Excel 2003 oder früheren Versionen gültig.(Geerbt von [`ChartFrame`](../chartframe/).) |
| virtual [Border](../../aspose.cells.charts/chartframe/border/) { get; } | Ruft den [`border`](../../aspose.cells.drawing/line/) ab. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultHeight](../../aspose.cells.charts/chartframe/defaultheight/) { get; } | (**Veraltet.**) Stellt die Höhe der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultHeightRatioToChart](../../aspose.cells.charts/chartframe/defaultheightratiotochart/) { get; } | Stellt die Höhe der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultWidth](../../aspose.cells.charts/chartframe/defaultwidth/) { get; } | (**Veraltet.**) Stellt die Breite der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultWidthRatioToChart](../../aspose.cells.charts/chartframe/defaultwidthratiotochart/) { get; } | Stellt die Breite der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultX](../../aspose.cells.charts/chartframe/defaultx/) { get; } | (**Veraltet.**) Stellt das x der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultXRatioToChart](../../aspose.cells.charts/chartframe/defaultxratiotochart/) { get; } | Stellt das x der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultY](../../aspose.cells.charts/chartframe/defaulty/) { get; } | (**Veraltet.**) Stellt das y der Standardposition in Einheiten von 1/4000 des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [DefaultYRatioToChart](../../aspose.cells.charts/chartframe/defaultyratiotochart/) { get; } | Stellt das y der Standardposition in Einheiten des Bruchteils des Diagrammbereichs dar. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [DirectionType](../../aspose.cells.charts/charttextframe/directiontype/) { get; set; } | Ruft die Richtung des Textes ab und legt sie fest. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| override [Font](../../aspose.cells.charts/displayunitlabel/font/) { get; } | Ruft ein [`Font`](./font/) Objekt des angegebenen ChartFrame-Objekts ab. |
| virtual [Height](../../aspose.cells.charts/chartframe/height/) { get; set; } | (**Veraltet.**) Ruft die Höhe des Rahmens ab oder legt sie fest in Einheiten von 1/4000 des Diagrammbereichs. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [HeightPixel](../../aspose.cells.charts/chartframe/heightpixel/) { get; set; } | Ruft die Höhe des Rahmens ab oder legt sie fest in Pixel‑Einheiten. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [HeightRatioToChart](../../aspose.cells.charts/chartframe/heightratiotochart/) { get; set; } | Ruft die Höhe des Rahmens ab oder legt sie fest in Einheiten des Verhältnisses zum Diagrammbereich. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [IsAutomaticRotation](../../aspose.cells.charts/charttextframe/isautomaticrotation/) { get; } | Gibt an, ob der Text des Diagramms automatisch gedreht wird. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsAutomaticSize](../../aspose.cells.charts/chartframe/isautomaticsize/) { get; set; } | Gibt an, ob der Diagrammrahmen automatisch dimensioniert wird. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [IsAutoText](../../aspose.cells.charts/charttextframe/isautotext/) { get; set; } | Gibt an, dass der Text automatisch erzeugt wird. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| [IsDefaultPosBeSet](../../aspose.cells.charts/chartframe/isdefaultposbeset/) { get; } | Gibt an, ob die Standardposition (DefaultX, DefaultY, DefaultWidth und DefaultHeight) festgelegt ist. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [IsDeleted](../../aspose.cells.charts/charttextframe/isdeleted/) { get; set; } | Gibt an, ob dieses Datenbeschriftungselement gelöscht wurde. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| [IsInnerMode](../../aspose.cells.charts/chartframe/isinnermode/) { get; set; } | Gibt an, ob die Größe des Plot‑Bereichs die Tick‑Markierungen und Achsenbeschriftungen einschließt. False bedeutet, dass die Größe die Größe des Plot‑Bereichs, der Tick‑Markierungen und der Achsenbeschriftungen bestimmen soll. (Vererbt von [`ChartFrame`](../chartframe/).) |
| [IsResizeShapeToFitText](../../aspose.cells.charts/charttextframe/isresizeshapetofittext/) { get; set; } | Ruft ab oder legt fest, ob eine Form automatisch angepasst werden soll, um den darin beschriebenen Text vollständig zu enthalten. Auto‑Fit bedeutet, dass der Text innerhalb einer Form skaliert wird, um den gesamten Text aufzunehmen. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [IsTextWrapped](../../aspose.cells.charts/charttextframe/istextwrapped/) { get; set; } | Ruft ab oder legt fest, ob der Text umbrochen wird. (Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [LinkedSource](../../aspose.cells.charts/charttextframe/linkedsource/) { get; set; } | Liest und schreibt eine Referenz auf das Arbeitsblatt.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| [ReadingOrder](../../aspose.cells.charts/charttextframe/readingorder/) { get; set; } | Stellt die Lesereihenfolge des Textes dar.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| [RotationAngle](../../aspose.cells.charts/charttextframe/rotationangle/) { get; set; } | Stellt den Drehwinkel des Textes dar.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| [Shadow](../../aspose.cells.charts/chartframe/shadow/) { get; set; } | Wahr, wenn der Rahmen einen Schatten hat.(Vererbt von [`ChartFrame`](../chartframe/).) |
| [ShapeProperties](../../aspose.cells.charts/chartframe/shapeproperties/) { get; } | Liest das [`ShapeProperties`](../chartframe/shapeproperties/) Objekt.(Vererbt von [`ChartFrame`](../chartframe/).) |
| override [Text](../../aspose.cells.charts/displayunitlabel/text/) { get; set; } | Liest oder legt fest den Text des Anzeigeeinheiten‑Labels. |
| [TextDirection](../../aspose.cells.charts/charttextframe/textdirection/) { get; set; } | (**Obsolete.**) Stellt die Lesereihenfolge des Textes dar.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextFont](../../aspose.cells.charts/chartframe/textfont/) { get; } | (**Obsolete.**) Liest ein [`Font`](../chartframe/font/) Objekt des angegebenen ChartFrame-Objekts.(Vererbt von [`ChartFrame`](../chartframe/).) |
| [TextHorizontalAlignment](../../aspose.cells.charts/charttextframe/texthorizontalalignment/) { get; set; } | Liest und schreibt die horizontale Ausrichtung des Textes.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [TextOptions](../../aspose.cells.charts/chartframe/textoptions/) { get; } | Liest und schreibt die Optionen des Textes.(Vererbt von [`ChartFrame`](../chartframe/).) |
| [TextVerticalAlignment](../../aspose.cells.charts/charttextframe/textverticalalignment/) { get; set; } | Liest oder schreibt die vertikale Ausrichtung des Textes.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [Width](../../aspose.cells.charts/chartframe/width/) { get; set; } | (**Obsolete.**) Liest oder schreibt die Breite des Rahmens in Einheiten von 1/4000 des Diagrammbereichs.(Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [WidthPixel](../../aspose.cells.charts/chartframe/widthpixel/) { get; set; } | Liest oder schreibt die Breite des Rahmens in Pixeln.(Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [WidthRatioToChart](../../aspose.cells.charts/chartframe/widthratiotochart/) { get; set; } | Liest oder schreibt die Breite des Rahmens als Verhältnis zum Diagrammbereich.(Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [X](../../aspose.cells.charts/chartframe/x/) { get; set; } | (**Obsolete.**) Liest oder legt fest die x‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [XPixel](../../aspose.cells.charts/chartframe/xpixel/) { get; set; } | Liest oder schreibt die X‑Koordinate der oberen linken Ecke in Pixeln.(Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [XRatioToChart](../../aspose.cells.charts/chartframe/xratiotochart/) { get; set; } | Liest oder legt fest die x‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [Y](../../aspose.cells.charts/chartframe/y/) { get; set; } | (**Obsolete.**) Liest oder legt fest die y‑Koordinate der oberen linken Ecke in Einheiten von 1/4000 des Diagrammbereichs. (Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [YPixel](../../aspose.cells.charts/chartframe/ypixel/) { get; set; } | Liest oder schreibt die Y‑Koordinate der oberen linken Ecke in Pixeln.(Vererbt von [`ChartFrame`](../chartframe/).) |
| virtual [YRatioToChart](../../aspose.cells.charts/chartframe/yratiotochart/) { get; set; } | Liest oder legt fest die y‑Koordinate der oberen linken Ecke in Einheiten des Verhältnisses zum Diagrammbereich. (Vererbt von [`ChartFrame`](../chartframe/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Characters](../../aspose.cells.charts/charttextframe/characters/)(int, int) | Gibt ein Characters‑Objekt zurück, das einen Zeichenbereich im Text darstellt.(Vererbt von [`ChartTextFrame`](../charttextframe/).) |
| virtual [SetPositionAuto](../../aspose.cells.charts/chartframe/setpositionauto/)() | Setzt die Position des Rahmens auf automatisch.(Vererbt von [`ChartFrame`](../chartframe/).) |

### Beispiele

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
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            // Hinzufügen eines neuen Arbeitsblatts zum Workbook-Objekt
            int sheetIndex = workbook.Worksheets.Add();
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Hinzufügen von Beispielwerten zu Zellen
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

            // Hinzufügen eines Diagramms zum Arbeitsblatt
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            // Zugriff auf die Instanz des neu hinzugefügten Diagramms
            Chart chart = worksheet.Charts[chartIndex];
            // Hinzufügen von NSeries (Diagrammdatenquelle) zum Diagramm vom Feld "A1" bis "B4"
            chart.NSeries.Add("A1:B4", true);
            // Festlegen der Datenquelle für die Kategoriedaten von NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Festlegen der Anzeigeeinheit der Werte‑(Y‑)Achse
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Festlegen von Eigenschaften des DisplayUnitLabel
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

            // Die Excel-Datei speichern
            workbook.Save("DisplayUnitLabelExample.xlsx");
            workbook.Save("DisplayUnitLabelExample.pdf");
        }
    }
}
```

### Siehe auch

* class [ChartTextFrame](../charttextframe/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


