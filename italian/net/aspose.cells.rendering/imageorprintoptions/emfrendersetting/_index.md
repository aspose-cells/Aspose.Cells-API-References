---
title: "ImageOrPrintOptions.EmfRenderSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Impostazione per il rendering dei metafile Emf nel file sorgente"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/emfrendersetting/
---
## ImageOrPrintOptions.EmfRenderSetting property

Impostazione per il rendering dei metafile EMF nel file sorgente.

```csharp
public EmfRenderSetting EmfRenderSetting { get; set; }
```

### Osservazioni

I metafile EMF identificati come "EMF+ Dual" possono contenere sia record EMF+ sia record EMF. Entrambi i tipi di record possono essere usati per renderizzare l'immagine, solo record EMF+, o solo record EMF. Quando EmfPlusPrefer è impostato, i record EMF+ verranno analizzati durante il rendering dell'immagine, altrimenti verranno analizzati solo i record EMF. Il valore predefinito è EmfOnly. Per i framework che dipendono da .NET System.Drawing.Common, questa impostazione viene ignorata.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing; // Added missing namespace AsposeCellsExamples
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyEmfRenderSettingDemo
    {
        public static void Run()
        {
            // Creare una nuova cartella di lavoro con contenuto di test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "EMF Rendering Setting Test";
            worksheet.Cells["C5"].Value = "Sample Content for Image Rendering";

            // Creare le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Tiff;
            options.TiffCompression = TiffCompression.CompressionLZW;

            // Visualizzare l'impostazione corrente
            Console.WriteLine("Default EmfRenderSetting: " + options.EmfRenderSetting);

            // Eseguire il rendering con le impostazioni EMF predefinite
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "DefaultEmfSetting.tiff");

            // Modifica l'impostazione di rendering EMF e renderizza nuovamente
            options.EmfRenderSetting = EmfRenderSetting.EmfPlusPrefer;
            Console.WriteLine("\nModified EmfRenderSetting: " + options.EmfRenderSetting);

            SheetRender modifiedRenderer = new SheetRender(worksheet, options);
            modifiedRenderer.ToImage(0, "ModifiedEmfSetting.tiff");

            Console.WriteLine("\nGenerated TIFF images demonstrating EMF rendering settings.");
        }
    }
}
```

### Vedi anche

* enum [EmfRenderSetting](../../../aspose.cells/emfrendersetting/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


