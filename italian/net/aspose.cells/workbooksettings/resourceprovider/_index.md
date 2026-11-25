---
title: "WorkbookSettings.ResourceProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà WorkbookSettings. Ottiene e imposta il provider di stream per risorse esterne, come il caricamento dei dati immagine per un'immagine di tipo LinkToFile"
type: docs
url: /it/net/aspose.cells/workbooksettings/resourceprovider/
---
## WorkbookSettings.ResourceProvider property

Ottiene e imposta il provider di stream per risorse esterne, come il caricamento dei dati immagine per un'immagine di tipo "LinkToFile".

```csharp
public IStreamProvider ResourceProvider { get; set; }
```

### Esempi

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
            // Crea una cartella di lavoro di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungere una forma di esempio per dimostrare il provider di risorse
            worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
            
            // Impostare il provider di risorse
            workbook.Settings.ResourceProvider = new MemoryStreamProvider();
            
            // Salvare la forma come immagine usando il provider di risorse
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

### Vedi anche

* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


