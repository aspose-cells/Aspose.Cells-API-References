---
title: "WorkbookRender.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorkbookRender. Renderiza todo el libro de trabajo como Imagen Tiff a un flujo"
type: docs
url: /es/net/aspose.cells.rendering/workbookrender/toimage/
---
## ToImage(Stream) {#toimage_3}

Renderizar todo el libro de trabajo como imagen Tiff a un flujo.

```csharp
public void ToImage(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | el flujo de la imagen de salida |

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Aspose.Cells ToImage Stream Demo";

            // Configurar opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png; // Fixed namespace AsposeCellsExamples

            // Crear el directorio de salida si no existe
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            // Crear un flujo de archivo para la salida de imagen
            string imagePath = Path.Combine(outputDir, "workbook_render.png");
            using (FileStream imageStream = new FileStream(imagePath, FileMode.Create))
            {
                try
                {
                    // Inicializar el renderizador de libro de trabajo y convertir a imagen
                    WorkbookRender renderer = new WorkbookRender(workbook, options); // Removed using statement
                    renderer.ToImage(imageStream);

                    Console.WriteLine($"Workbook rendered successfully to: {imagePath}");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error during rendering: {ex.Message}");
                }
            }

            // Guardar el libro de trabajo original como referencia
            workbook.Save(Path.Combine(outputDir, "source_workbook.xlsx"));
        }
    }
}
```

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(string) {#toimage_4}

Renderizar todo el libro de trabajo como imagen Tiff a un archivo.

```csharp
public void ToImage(string filename)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | String | el nombre de archivo de la imagen de salida |

### Ejemplos

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
            // Crear un libro de trabajo de ejemplo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("Test ToImage Method");
            
            // Establezca opciones de imagen
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.ImageType = ImageType.Tiff;
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;

            // Crear renderizado del libro de trabajo y guardar como imagen
            WorkbookRender wbRender = new WorkbookRender(wb, imgOpt);
            string outputPath = "output.tiff";
            wbRender.ToImage(outputPath);
            
            Console.WriteLine("Workbook rendered to image: " + outputPath);
        }
    }
}
```

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_2}

Renderizar una página específica a un archivo.

```csharp
public void ToImage(int pageIndex, string fileName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| fileName | String | nombre de archivo de la imagen de salida |

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                OnePagePerSheet = true
            };

            // Crear renderizador de libro de trabajo
            WorkbookRender renderer = new WorkbookRender(workbook, options);

            // Guardar cada página como imagen
            for (int i = 0; i < renderer.PageCount; i++)
            {
                renderer.ToImage(i, $"output_page_{i}.png");
            }
        }
    }
}
```

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_1}

Renderizar una página específica a un flujo.

```csharp
public void ToImage(int pageIndex, Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| stream | Stream | el flujo de la imagen de salida |

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index and Stream Demo";

            // Configurar opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;

            try
            {
                // Inicializar el renderizador de libro de trabajo
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Obtener el índice de la primera página (basado en 0)
                int pageIndex = 0;

                // Crear un flujo de memoria para contener la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llamar a ToImage con el índice de página y el flujo
                    renderer.ToImage(pageIndex, stream);

                    // Mostrar resultados
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

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int) {#toimage}

Renderizar una página específica a un objeto Bitmap.

```csharp
public Bitmap ToImage(int pageIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |

### Valor de retorno

el objeto bitmap de la página

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "ToImage with Page Index Demo";

            // Configurar opciones de renderizado de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

            // Crear el directorio de salida si no existe
            string outputDir = "output/";
            Directory.CreateDirectory(outputDir);

            try
            {
                // Inicializar el renderizador de libro de trabajo
                WorkbookRender renderer = new WorkbookRender(workbook, options);

                // Obtener el índice de la primera página (basado en 0)
                int pageIndex = 0;

                // Llamar a ToImage con el índice de página y guardar en archivo
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

### Ver también

* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


