---
title: "ImageOrPrintOptions.IsCellAutoFit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Indica se la larghezza e l'altezza delle celle sono adattate automaticamente al valore della cella. Il valore predefinito è false"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/iscellautofit/
---
## ImageOrPrintOptions.IsCellAutoFit property

Indica se la larghezza e l'altezza delle celle sono adattate automaticamente al valore della cella. Il valore predefinito è false.

```csharp
[Obsolete("This property is not used, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCellAutoFit { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, questa proprietà non è utilizzata, si prega di rimuovere questa proprietà. Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyIsCellAutoFitDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta un testo di esempio che supera la larghezza predefinita della colonna
            worksheet.Cells["B4"].Value = "This is a long text that demonstrates cell autofit behavior when converting to image.";
            
            // Creare le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            
            // Dimostra IsCellAutoFit false (predefinito)
            Console.WriteLine("Default IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithoutAutoFit.png");

            // Modifica IsCellAutoFit a true
            options.IsCellAutoFit = true;
            Console.WriteLine("Modified IsCellAutoFit value: " + options.IsCellAutoFit);
            SaveAsImage(worksheet, options, "WithAutoFit.png");

            Console.WriteLine("Images created successfully. Compare column widths in output files.");
        }

        private static void SaveAsImage(Worksheet worksheet, ImageOrPrintOptions options, string fileName)
        {
            // Configura il formato immagine
            options.ImageType = ImageType.Png;

            // Esegui il rendering del foglio di lavoro in immagine con le opzioni specificate
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, fileName);
        }
    }
}
```

### Vedi anche

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


