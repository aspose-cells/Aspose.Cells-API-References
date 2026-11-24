---
title: "ImageOrPrintOptions.PrintWithStatusDialog"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Wenn PrintWithStatusDialog true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt; andernfalls wird kein solcher Dialog angezeigt."
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/
---
## ImageOrPrintOptions.PrintWithStatusDialog property

Wenn PrintWithStatusDialog = true ist, wird ein Dialog angezeigt, der den aktuellen Druckstatus zeigt. Andernfalls wird kein solcher Dialog angezeigt.

```csharp
public bool PrintWithStatusDialog { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using System.Threading;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPrintWithStatusDialogDemo
    {
        public static void Run()
        {
            // Initialisiere eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Bild- oder Druckoptionen festlegen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.PrintWithStatusDialog = false; // Disable print status dialog
            options.PageIndex = 0;
            options.PageCount = 1;

            // SheetRender erstellen
            SheetRender sheetRender = new SheetRender(worksheet, options);
            
            // In PDF drucken
            sheetRender.ToImage(0, "output.png");

            // Warte auf Dateierstellung (vereinfachte Warte‑Logik)
            int attempts = 0;
            while (!File.Exists("output.png") && attempts < 5)
            {
                Thread.Sleep(1000);
                attempts++;
            }

            if (File.Exists("output.png"))
            {
                Console.WriteLine("Image file created successfully");
            }
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


