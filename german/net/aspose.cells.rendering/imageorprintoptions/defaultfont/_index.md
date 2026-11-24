---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Wenn Zeichen in Excel Unicode sind und im Zellenstil nicht mit der richtigen Schriftart festgelegt wurden, können sie im pdfimage als Block erscheinen. Setze die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht gesetzt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie die DefaultFont, z. B. MingLiu oder MS Gothic, um diese Zeichen anzuzeigen. Wenn diese Eigenschaft nicht festgelegt ist, verwendet Aspose.Cells die systemweite Standardschriftart, um diese Unicode‑Zeichen darzustellen.

```csharp
public string DefaultFont { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieltext zur Zelle hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // Erstelle Bildoptionen und setze die Standardschriftart
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // Render das Arbeitsblatt zu einem Bild
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


