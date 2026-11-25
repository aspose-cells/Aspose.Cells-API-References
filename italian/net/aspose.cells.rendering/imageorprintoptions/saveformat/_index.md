---
title: "ImageOrPrintOptions.SaveFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta il tipo di formato file di output. Supporta Tiff/XPS"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/saveformat/
---
## ImageOrPrintOptions.SaveFormat property

Ottiene o imposta il tipo di formato file di output. Supporta Tiff/XPS

```csharp
[Obsolete("For Tiff/Svg, use ImageType; For Xps, use Workbook.Save(string, SaveOptions) with XpsSaveOptions")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SaveFormat SaveFormat { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, per Tiff/Svg, usa [`ImageType`](../imagetype/); per Xps, usa [`Save`](../../../aspose.cells/workbook/save/) con [`XpsSaveOptions`](../../../aspose.cells/xpssaveoptions/). Questa proprietà sarà rimossa tra 12 mesi a partire da agosto 2022. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e popola con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells SaveFormat Demonstration");
            
            // Crea un'istanza di ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();

            // Visualizza il valore iniziale di SaveFormat
            Console.WriteLine("Initial SaveFormat: " + options.SaveFormat);

            // Imposta SaveFormat su TIFF e renderizza il foglio di lavoro
            options.SaveFormat = SaveFormat.Tiff;
            SheetRender tiffRenderer = new SheetRender(worksheet, options);
            using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
            {
                tiffRenderer.ToTiff(tiffStream);
            }
            Console.WriteLine("Rendered worksheet to TIFF format");

            // Cambia SaveFormat in XPS e renderizza nuovamente
            options.SaveFormat = SaveFormat.Xps;
            SheetRender xpsRenderer = new SheetRender(worksheet, options);
            using (FileStream xpsStream = new FileStream("output.xps", FileMode.Create))
            {
                // Nota: SheetRender non supporta il formato XPS. Questo verrà salvato invece come formato immagine.
                xpsRenderer.ToImage(0, xpsStream);
            }
            Console.WriteLine("Rendered worksheet to XPS format");
        }
    }
}
```

### Vedi anche

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


