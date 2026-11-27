---
title: "WorkbookSettings.ResourceProvider"
second_title: "Aspose.Cells för .NET API‑referens"
description: "WorkbookSettings property. Hämtar och sätter strömtillhandahållaren för externa resurser, såsom att ladda bilddata för bild av typen LinkToFile"
type: docs
url: /sv/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Hämtar och anger strömleverantören för extern resurs, såsom att ladda bilddata för bild av typen "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Exempel

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
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett exempel på form för att demonstrera resursleverantören
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Ställ in resursleverantören
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Spara formen som bild med hjälp av resursleverantören
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

### Se även

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


