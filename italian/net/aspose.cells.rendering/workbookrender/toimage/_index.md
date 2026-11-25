---
title: "WorkbookRender.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo WorkbookRender. Renderizza l'intera cartella di lavoro come immagine Tiff in stream"
type: docs
url: /it/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Esegui il rendering dell'intera cartella di lavoro come immagine Tiff in uno stream.

```csharp
public void ToImage(Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| stream | Stream | lo stream dell'immagine di output |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithStreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Configura le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Crea la directory di output se non esiste
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Crea un flusso di file per l'output dell'immagine
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Inizializza il workbook renderer e convertilo in immagine
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Salva la cartella di lavoro originale per riferimento
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Esegui il rendering dell'intera cartella di lavoro come immagine Tiff in un file.

```csharp
public void ToImage(string filename)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filename | String | il nome file dell'immagine di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithStringDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro di esempio
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Imposta le opzioni dell'immagine
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Crea workbook render e salva come immagine
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Esegui il rendering di una pagina specifica in un file.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| fileName | String | nome file dell'immagine di output |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Crea il renderer della cartella di lavoro
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Salva ogni pagina come immagine
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Esegui il rendering di una pagina specifica in uno stream.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| stream | Stream | lo stream dell'immagine di output |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Configura le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Inizializza il workbook renderer
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Ottieni l'indice della prima pagina (basato su 0)
                int pageIndex = 0;

                // Crea un flusso di memoria per contenere l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama ToImage con l'indice della pagina e lo stream
                    renderer.ToImage(pageIndex, stream);

                    // Visualizza i risultati
                    Console.WriteLine($"Page {pageIndex} rendered successfully to stream");
                    Console.WriteLine($"Stream length: {stream.Length} bytes");
                    Console.WriteLine($"Total pages available: {renderer.PageCount}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Esegui il rendering di una pagina specifica in un oggetto Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |

### Valore di ritorno

l'oggetto bitmap della pagina

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class WorkbookRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Configura le opzioni di rendering dell'immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Crea la directory di output se non esiste
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Inizializza il workbook renderer
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Ottieni l'indice della prima pagina (basato su 0)
                int pageIndex = 0;

                // Chiama ToImage con l'indice della pagina e salva su file
                string imagePath = Path.Combine(outputDir, $"page_{pageIndex}.png");
                renderer.ToImage(pageIndex, imagePath);

                Console.WriteLine($"Page {pageIndex} rendered successfully to: {imagePath}");
                Console.WriteLine($"Total pages available: {renderer.PageCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


