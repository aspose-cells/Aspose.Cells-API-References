---
title: "Klasse RenderingWatermark"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.RenderingWatermark-Klasse. Wasserzeichen für das Rendering"
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/
---
## RenderingWatermark class

Wasserzeichen für das Rendern.

```csharp
public class RenderingWatermark
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [RenderingWatermark](renderingwatermark/#constructor)(byte[]) | Erstellt eine Instanz eines Bildwasserzeichens. |
| [RenderingWatermark](renderingwatermark/#constructor_1)(string, RenderingFont) | Erstellt eine Instanz eines Textwasserzeichens. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Font](../../aspose.cells.rendering/renderingwatermark/font/) { get; } | Liest die Schriftart des Wasserzeichens. |
| [HAlignment](../../aspose.cells.rendering/renderingwatermark/halignment/) { get; set; } | Liest oder setzt die horizontale Ausrichtung des Wasserzeichens zur Seite. |
| [Image](../../aspose.cells.rendering/renderingwatermark/image/) { get; } | Liest das Bild des Wasserzeichens. |
| [IsBackground](../../aspose.cells.rendering/renderingwatermark/isbackground/) { get; set; } | Gibt an, ob das Wasserzeichen hinter dem Seiteninhalt platziert wird. |
| [OffsetX](../../aspose.cells.rendering/renderingwatermark/offsetx/) { get; set; } | Liest oder setzt den Versatzwert für [`HAlignment`](./halignment/) |
| [OffsetY](../../aspose.cells.rendering/renderingwatermark/offsety/) { get; set; } | Liest oder setzt den Versatzwert für [`VAlignment`](./valignment/) |
| [Opacity](../../aspose.cells.rendering/renderingwatermark/opacity/) { get; set; } | Liest oder setzt die Deckkraft des Wasserzeichens im Bereich [0, 1]. |
| [Rotation](../../aspose.cells.rendering/renderingwatermark/rotation/) { get; set; } | Liest oder setzt die Drehung des Wasserzeichens in Grad. |
| [ScaleToPagePercent](../../aspose.cells.rendering/renderingwatermark/scaletopagepercent/) { get; set; } | Liest oder setzt die Skalierung relativ zur Zielseite in Prozent. |
| [Text](../../aspose.cells.rendering/renderingwatermark/text/) { get; } | Liest den Text des Wasserzeichens. |
| [VAlignment](../../aspose.cells.rendering/renderingwatermark/valignment/) { get; set; } | Liest oder setzt die vertikale Ausrichtung des Wasserzeichens zur Seite. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Drawing;

    public class RenderingWatermarkDemo
    {
        public static void RenderingWatermarkExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("This is a sample worksheet.");

            // Erstelle eine Schriftart für das Wasserzeichen
            RenderingFont font = new RenderingFont("Calibri", 68);
            font.Italic = true;
            font.Bold = true;
            font.Color = Color.Blue;

            // Erstelle ein Wasserzeichen aus Text und der angegebenen Schriftart
            RenderingWatermark watermark = new RenderingWatermark("Watermark", font);

            // Lege Eigenschaften für das Wasserzeichen fest
            watermark.HAlignment = TextAlignmentType.Center;
            watermark.VAlignment = TextAlignmentType.Center;
            watermark.Rotation = 30;
            watermark.Opacity = 0.6f;
            watermark.ScaleToPagePercent = 50;
            watermark.IsBackground = true;

            // Gib das Wasserzeichen für die PDF-Renderung an
            PdfSaveOptions options = new PdfSaveOptions();
            options.Watermark = watermark;

            // Speichere die Arbeitsmappe als PDF mit dem Wasserzeichen
            workbook.Save("output_watermark.pdf", options);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


