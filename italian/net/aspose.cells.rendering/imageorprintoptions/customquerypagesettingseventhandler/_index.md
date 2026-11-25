---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Il client può controllare le impostazioni di pagina della stampante quando stampa ogni pagina usando questo EventHandler"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

Il client può controllare le impostazioni di pagina della stampante quando stampa ogni pagina utilizzando questo EventHandler

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visualizza alcune delle proprietà disponibili
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Dimostra l'impostazione di alcune proprietà
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Verifica che le proprietà siano impostate
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // Crea un SheetRender per dimostrare il rendering
                SheetRender renderer = new SheetRender(worksheet, options);

                // Salva la cartella di lavoro
                workbook.Save("CustomQueryPageSettingsEventHandlerDemo.xlsx");

                Console.WriteLine("ImageOrPrintOptions demonstration completed");
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


