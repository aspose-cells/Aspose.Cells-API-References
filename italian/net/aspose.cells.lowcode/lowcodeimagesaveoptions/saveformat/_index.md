---
title: "LowCodeImageSaveOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LowCodeImageSaveOptions. Ottiene o imposta il formato di salvataggio"
type: docs
url: /it/net/aspose.cells.lowcode/lowcodeimagesaveoptions/saveformat/
---
## LowCodeImageSaveOptions.SaveFormat property

Ottiene o imposta il formato di salvataggio.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### Osservazioni

Se [`ImageOptions`](../imageoptions/) è stato specificato, impostare questa proprietà cambierà anche il valore di [`ImageType`](../../../aspose.cells.rendering/imageorprintoptions/imagetype/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeImageSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells LowCode Image SaveFormat Demo");

            // Inizializza LowCodeImageSaveOptions con i valori predefiniti
            LowCodeImageSaveOptions options = new LowCodeImageSaveOptions();
            
            // Visualizza il SaveFormat iniziale (il valore predefinito è Png)
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Configura per l'output JPEG
            options.SaveFormat = SaveFormat.Jpg;
            options.ImageOptions = new ImageOrPrintOptions
            {
                Quality = 85,
                OnePagePerSheet = true,
                ImageType = ImageType.Jpeg
            };
            SaveWorksheetAsImage(worksheet, options, "output_initial.jpg");

            // Cambia al formato PNG e salva di nuovo
            options.SaveFormat = SaveFormat.Png;
            options.ImageOptions.ImageType = ImageType.Png;
            Console.WriteLine("\nModified SaveFormat: " + options.SaveFormat);
            SaveWorksheetAsImage(worksheet, options, "output_modified.png");
        }

        private static void SaveWorksheetAsImage(Worksheet worksheet, LowCodeImageSaveOptions options, string fileName)
        {
            // Esegui il rendering del foglio di lavoro usando le opzioni configurate
            SheetRender renderer = new SheetRender(worksheet, options.ImageOptions);
            renderer.ToImage(0, fileName);
            Console.WriteLine($"Saved: {fileName}");
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeImageSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


