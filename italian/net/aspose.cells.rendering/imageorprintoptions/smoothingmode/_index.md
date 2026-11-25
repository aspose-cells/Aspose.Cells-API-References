---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Specifica se l'anti-aliasing di smoothing è applicato a linee e curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Specifica se la smussatura (anti-aliasing) viene applicata a linee e curve e ai bordi delle aree riempite. Il valore predefinito è SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visualizza alcune delle proprietà disponibili
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Crea un SheetRender per dimostrare la proprietà
                SheetRender renderer = new SheetRender(worksheet, options);

                // Esegui il rendering su uno stream di memoria per dimostrare la funzionalità
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Salva la cartella di lavoro
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


