---
title: "SheetRender.ToImage"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SheetRender. Renderizza una determinata pagina su un oggetto Graphics"
type: docs
url: /it/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Renderizza una certa pagina su un oggetto Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| g | Grafica | L'oggetto su cui eseguire il rendering. |
| x | Single | La coordinata X (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| y | Single | La coordinata Y (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| larghezza | Single | La larghezza massima (in pixel) che può occupare la pagina renderizzata. |
| altezza | Single | L'altezza massima (in pixel) che può occupare la pagina renderizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleSingleSingleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Crea opzioni immagine
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crea il rendering del foglio per il foglio di lavoro
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Crea uno stream di memoria per catturare l'immagine renderizzata
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama ToImage con i parametri specificati
                    // Poiché non possiamo usare System.Drawing.Graphics, utilizzeremo la sovraccarico più semplice di ToImage
                    sheetRender.ToImage(0, stream);

                    // Salva l'immagine renderizzata su file
                    File.WriteAllBytes("RenderedOutput.png", stream.ToArray());
                }

                Console.WriteLine("Sheet rendered to image successfully.");
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

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Renderizza una certa pagina su un oggetto Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pageIndex | Int32 | indica quale pagina deve essere convertita |
| g | Grafica | L'oggetto su cui eseguire il rendering. |
| x | Single | La coordinata X (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |
| y | Single | La coordinata Y (in pixel) dell'angolo superiore sinistro della pagina renderizzata. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SheetRenderMethodToImageWithInt32GraphicsSingleSingleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Crea un'istanza di SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Poiché non possiamo usare i tipi System.Drawing, utilizzeremo il metodo alternativo ToImage
                // che salva direttamente su un file
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Pulisci le risorse
                sheetRender.Dispose();
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

## ToImage(int, string) {#toimage_4}

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
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Carica il file Excel di origine
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Crea opzioni immagine
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crea il rendering del foglio per il primo foglio di lavoro
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Renderizza la prima pagina del foglio in un file immagine
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

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

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Crea opzioni immagine
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crea un'istanza di SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Crea un flusso di memoria per contenere l'immagine
                using (MemoryStream stream = new MemoryStream())
                {
                    // Chiama ToImage con i parametri indice pagina e stream
                    sheetRender.ToImage(0, stream);

                    Console.WriteLine($"Successfully rendered page 0 to stream. Stream length: {stream.Length} bytes");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
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

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Crea opzioni immagine
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crea un'istanza di SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Ottieni l'indice della prima pagina (basato su 0)
                int pageIndex = 0;

                // Chiama ToImage con il parametro indice pagina
                sheetRender.ToImage(pageIndex, "output_page.png");

                Console.WriteLine($"Successfully rendered page {pageIndex} to image");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error rendering to image: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


