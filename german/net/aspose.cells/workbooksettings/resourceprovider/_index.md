---
title: "WorkbookSettings.ResourceProvider"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookSettings-Eigenschaft. Gibt den Stream-Anbieter für externe Ressourcen zurück und setzt ihn, z. B. zum Laden von Bilddaten für ein Bild vom Typ LinkToFile"
type: docs
url: /de/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Liest und setzt den Stream‑Provider für externe Ressourcen, z. B. das Laden von Bilddaten für ein Bild vom Typ "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyResourceProviderDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie eine Beispielform hinzu, um den Ressourcenanbieter zu demonstrieren
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Ressourcenanbieter festlegen
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Speichern Sie die Form als Bild unter Verwendung des Ressourcenanbieters
            string outputPath = "output_shape.png";
            worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
            
            Console.WriteLine("Shape saved as image using ResourceProvider.");
        }
    }

    public class MemoryStreamProvider : IStreamProvider
    {
        public void CloseStream(StreamProviderOptions options)
        {
            options.Stream.Close();
        }

        public void InitStream(StreamProviderOptions options)
        {
            options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
        }
    }
}
```

### Siehe auch

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


