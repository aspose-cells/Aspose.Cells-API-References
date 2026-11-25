---
title: "ImageOrPrintOptions.CustomPrintPageEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Il client può inviare output speciale alla stampante quando stampa ogni pagina utilizzando questo EventHandler"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

Il client può inviare output speciale alla stampante quando stampa ogni pagina utilizzando questo EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data for Printing";
            worksheet.Cells["A2"].Value = "This demonstrates printing options";

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Configura le opzioni di stampa
                options.PrintWithStatusDialog = true;
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;

                // Visualizzare le opzioni di stampa correnti
                Console.WriteLine($"PrintWithStatusDialog: {options.PrintWithStatusDialog}");
                Console.WriteLine($"HorizontalResolution: {options.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {options.VerticalResolution}");

                // Creare un SheetRender per dimostrare la stampa
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Esegui il rendering in immagine per dimostrare la stampa
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Rendering completed successfully.");
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


