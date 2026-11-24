---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Wenn Zeichen in Excel Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie im pdfimage als Block erscheinen. Setzen Sie dies auf true, um zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

Wenn Zeichen in der Excel-Datei Unicode sind und nicht mit der richtigen Schriftart im Zellenstil festgelegt wurden, können sie als Block in PDF oder Bild erscheinen. Setzen Sie diesen Wert auf true, um zunächst zu versuchen, die Standardschriftart der Arbeitsmappe zu verwenden, um diese Zeichen anzuzeigen.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Hinweise

Standard ist true.

### Beispiele

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Legen Sie die Standardschriftart für die Arbeitsmappe fest
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Bild- oder Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Aktivieren Sie die Überprüfung der Standardschriftart der Arbeitsmappe
            options.CheckWorkbookDefaultFont = true;

            // Render das Arbeitsblatt zu einem Bild
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Speichere das Bild in einer Datei
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


