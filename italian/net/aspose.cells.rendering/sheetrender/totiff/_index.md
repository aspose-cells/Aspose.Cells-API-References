---
title: "SheetRender.ToTiff"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SheetRender. Renderizza l'intero worksheet come immagine Tiff nello stream"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Renderizza l'intero foglio di lavoro come immagine Tiff nello stream.

```csharp
public void ToTiff(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | lo stream dell'immagine di output |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToTiffWithStreamDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungere contenuto di esempio per dimostrare il rendering
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Configurare le opzioni immagine per il rendering
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Creare il renderer del foglio con le opzioni configurate
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Creare lo stream di output per l'immagine TIFF
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Renderizzare il worksheet in TIFF usando lo stream
                    renderer.ToTiff(tiffStream);
                    Console.WriteLine("Worksheet successfully rendered to TIFF stream.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during TIFF rendering: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Renderizza l'intero foglio di lavoro come immagine Tiff in un file.

```csharp
public void ToTiff(string filename)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filename | String | il nome file dell'immagine di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodToTiffWithStringDemo
    {
        public static void Run()
        {
            // Carica il file Excel di origine
            Workbook workbook = new Workbook("Book1.xlsx");

            // Crea opzioni di immagine o stampa
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Crea il rendering del foglio per il primo foglio di lavoro
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Salvare tutte le pagine del foglio come file TIFF multipagina
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


