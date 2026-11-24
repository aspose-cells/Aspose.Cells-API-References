---
title: "Klasse MsoFormatPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.MsoFormatPicture Klasse. Stellt das Bildformat dar"
type: docs
url: /de/net/aspose.cells.drawing/msoformatpicture/
---
## MsoFormatPicture class

Stellt das Bildformat dar.

```csharp
public class MsoFormatPicture
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [BottomCrop](../../aspose.cells.drawing/msoformatpicture/bottomcrop/) { get; set; } | Stellt die Position des unteren Randes des Beschnittrechtecks dar, ausgedrückt als Verhältnis zur Bildhöhe. |
| [BottomCropInch](../../aspose.cells.drawing/msoformatpicture/bottomcropinch/) { get; set; } | Stellt die Position des unteren Randes des Beschnittrechtecks dar, in Zoll. |
| [Brightness](../../aspose.cells.drawing/msoformatpicture/brightness/) { get; set; } | Stellt die Helligkeitsänderung für das Bild in Prozent dar. |
| [Contrast](../../aspose.cells.drawing/msoformatpicture/contrast/) { get; set; } | Stellt die Kontraständerung für das Bild in Prozent dar. |
| [Gamma](../../aspose.cells.drawing/msoformatpicture/gamma/) { get; set; } | Stellt das Gamma des Bildes dar. |
| [IsBiLevel](../../aspose.cells.drawing/msoformatpicture/isbilevel/) { get; set; } | Gibt an, ob dieses Bild in zweifarbigen Schwarz‑Weiß angezeigt werden soll. |
| [IsGray](../../aspose.cells.drawing/msoformatpicture/isgray/) { get; set; } | Gibt an, ob dieses Bild in Graustufen angezeigt werden soll. |
| [LeftCrop](../../aspose.cells.drawing/msoformatpicture/leftcrop/) { get; set; } | Stellt die Position der linken Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildbreite. |
| [LeftCropInch](../../aspose.cells.drawing/msoformatpicture/leftcropinch/) { get; set; } | Stellt die Position der linken Seite des Zuschneide‑Rechtecks dar, in Zoll. |
| [RightCrop](../../aspose.cells.drawing/msoformatpicture/rightcrop/) { get; set; } | Stellt die Position der rechten Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildbreite. |
| [RightCropInch](../../aspose.cells.drawing/msoformatpicture/rightcropinch/) { get; set; } | Stellt die Position der rechten Seite des Zuschneide‑Rechtecks dar, in Zoll. |
| [TopCrop](../../aspose.cells.drawing/msoformatpicture/topcrop/) { get; set; } | Stellt die Position der oberen Seite des Zuschneide‑Rechtecks dar, ausgedrückt als Verhältnis zur Bildhöhe. |
| [TopCropInch](../../aspose.cells.drawing/msoformatpicture/topcropinch/) { get; set; } | Stellt die Position der oberen Seite des Zuschneide‑Rechtecks dar, in Zoll. |
| [Transparency](../../aspose.cells.drawing/msoformatpicture/transparency/) { get; set; } | Gibt den Transparenzgrad des Bereichs zurück oder legt ihn fest, als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [TransparentColor](../../aspose.cells.drawing/msoformatpicture/transparentcolor/) { get; set; } | Liest und setzt die transparente Farbe des Bildes. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/msoformatpicture/equals/)(object) |  |
| override [GetHashCode](../../aspose.cells.drawing/msoformatpicture/gethashcode/)() | Liest den Hash‑Code. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPictureDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ein Bild zum Arbeitsblatt hinzufügen
            int pictureIndex = sheet.Pictures.Add(5, 5, "MsoFormatPictureDemo.jpg");
            Picture picture = sheet.Pictures[pictureIndex];

            // Greift auf das MsoFormatPicture‑Objekt zu
            MsoFormatPicture formatPicture = picture.FormatPicture;

            // Setzt Eigenschaften von MsoFormatPicture
            formatPicture.TopCropInch = 0.5;
            formatPicture.BottomCropInch = 0.5;
            formatPicture.LeftCropInch = 0.5;
            formatPicture.RightCropInch = 0.5;
            formatPicture.Transparency = 0.5;
            formatPicture.Contrast = 0.8;
            formatPicture.Brightness = 0.6;
            formatPicture.Gamma = 1.0;
            formatPicture.IsBiLevel = false;
            formatPicture.IsGray = false;

            // Setzt die transparente Farbe
            CellsColor transparentColor = workbook.CreateCellsColor();
            transparentColor.Color = Color.White;
            formatPicture.TransparentColor = transparentColor;

            // Speichere die Arbeitsmappe
            workbook.Save("MsoFormatPictureDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


