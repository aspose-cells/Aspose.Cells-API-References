---
title: "ImageOrPrintOptions.EmfType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta un EmfType che specifica il formato del Metafile. Il valore predefinito è EmfPlusDual"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/emftype/
---
## ImageOrPrintOptions.EmfType property

Ottiene o imposta un EmfType che specifica il formato del Metafile. Il valore predefinito è EmfPlusDual.

```csharp
public EmfType EmfType { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertyEmfTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "EMF Type Demo";

            try
            {
                // Crea un'istanza di ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Imposta il tipo di immagine su EMF
                options.ImageType = Aspose.Cells.Drawing.ImageType.Emf;

                // Crea SheetRender con le opzioni
                SheetRender renderer = new SheetRender(worksheet, options);

                // Salva in formato EMF
                using (MemoryStream stream = new MemoryStream())
                {
                    renderer.ToImage(0, stream);

                    // Visualizza il valore della proprietà EmfType
                    Console.WriteLine("EmfType value: " + options.EmfRenderSetting);

                    // Salva il file EMF
                    File.WriteAllBytes("output.emf", stream.ToArray());
                    Console.WriteLine("EMF file created successfully.");
                }
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


