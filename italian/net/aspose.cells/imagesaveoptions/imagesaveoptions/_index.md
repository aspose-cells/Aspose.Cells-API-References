---
title: "ImageSaveOptions.ImageSaveOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ImageSaveOptions. Crea le opzioni per salvare il file immagine"
type: docs
url: /it/net/aspose.cells/imagesaveoptions/imagesaveoptions/
---
## ImageSaveOptions() {#constructor}

Crea le opzioni per salvare il file immagine.

```csharp
public ImageSaveOptions()
```

### Osservazioni

Il tipo predefinito è Tiff.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ImageSaveOptionsMethodSharpctorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per il contesto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Dimostra il costruttore senza parametri
                ImageSaveOptions defaultOptions = new ImageSaveOptions();
                Console.WriteLine("Created ImageSaveOptions with default constructor");

                // Dimostra il costruttore con parametro SaveFormat
                ImageSaveOptions pngOptions = new ImageSaveOptions(SaveFormat.Png);
                Console.WriteLine("Created ImageSaveOptions with SaveFormat.Png");

                // Accedi alla proprietà di sola lettura ImageOrPrintOptions
                var imageOptions = pngOptions.ImageOrPrintOptions;
                Console.WriteLine($"ImageOrPrintOptions type: {imageOptions.GetType().Name}");

                // Imposta la proprietà StreamProvider
                pngOptions.StreamProvider = null;
                Console.WriteLine("StreamProvider set to null");

                // Salva la cartella di lavoro con le opzioni create
                workbook.Save("output.png", pngOptions);
                Console.WriteLine("Workbook saved successfully with ImageSaveOptions");
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

* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImageSaveOptions(SaveFormat) {#constructor_1}

Crea le opzioni per salvare il file immagine.

```csharp
public ImageSaveOptions(SaveFormat saveFormat)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| saveFormat | SaveFormat | Il formato del file. Deve essere uno dei seguenti tipi: Tiff, Svg, Bmp, Png, Jpg, Emf o Gif, altrimenti il formato salvato verrà impostato automaticamente a Tiff. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageSaveOptionsMethodCtorWithSaveFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook e aggiungi dati di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells Image Save Demo");
            
            // Crea ImageSaveOptions con SaveFormat.Tiff
            try
            {
                ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Tiff);
                
                // Configura le opzioni di rendering dell'immagine
                saveOptions.ImageOrPrintOptions.HorizontalResolution = 300;
                saveOptions.ImageOrPrintOptions.VerticalResolution = 300;

                // Salva il workbook come TIFF multipagina
                workbook.Save("WorksheetImage.tiff", saveOptions);
                
                Console.WriteLine("Workbook successfully saved as TIFF image with 300 DPI resolution.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during image save operation: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../saveformat/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


