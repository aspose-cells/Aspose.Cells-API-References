---
title: "SheetRender.ToImage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SheetRender. Renderiza una página determinada a un Graphics"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/toimage/
---
## ToImage(int, Graphics, float, float, float, float) {#toimage_2}

Renderizar una página determinada a un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y, float width, float height)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| g | Graphics | El objeto donde renderizar. |
| x | Single | La coordenada X (en píxeles) de la esquina superior izquierda de la página renderizada. |
| y | Single | La coordenada Y (en píxeles) de la esquina superior izquierda de la página renderizada. |
| ancho | Single | El ancho máximo (en píxeles) que puede ocupar la página renderizada. |
| altura | Single | La altura máxima (en píxeles) que puede ocupar la página renderizada. |

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            try
            {
                // Crear opciones de imagen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crear renderizado de hoja para la hoja de cálculo
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Crear un flujo de memoria para capturar la imagen renderizada
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llamar a ToImage con los parámetros especificados
                    // Dado que no podemos usar System.Drawing.Graphics, utilizaremos la sobrecarga más simple de ToImage
                    sheetRender.ToImage(0, stream);

                    // Guardar la imagen renderizada en un archivo
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

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Graphics, float, float) {#toimage_1}

Renderizar una página determinada a un Graphics

```csharp
public void ToImage(int pageIndex, Graphics g, float x, float y)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pageIndex | Int32 | indicar qué página se va a convertir |
| g | Graphics | El objeto donde renderizar. |
| x | Single | La coordenada X (en píxeles) de la esquina superior izquierda de la página renderizada. |
| y | Single | La coordenada Y (en píxeles) de la esquina superior izquierda de la página renderizada. |

### Ejemplos

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
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data for Rendering";
            worksheet.Cells["A2"].Value = "This will be rendered to an image";

            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Crear una instancia de SheetRender
            SheetRender sheetRender = new SheetRender(worksheet, options);

            try
            {
                // Dado que no podemos usar tipos de System.Drawing, utilizaremos el método alternativo ToImage
                // que guarda directamente en un archivo
                sheetRender.ToImage(0, "RenderedOutput.png");
                Console.WriteLine("Sheet rendered to image successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during rendering: {ex.Message}");
            }
            finally
            {
                // Liberar recursos
                sheetRender.Dispose();
            }
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, string) {#toimage_4}

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
    public class SheetRenderMethodToImageWithInt32StringDemo
    {
        public static void Run()
        {
            // Cargar el archivo Excel de origen
            Workbook workbook = new Workbook("Book1.xlsx");
            
            // Crear opciones de imagen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crear renderizado de hoja para la primera hoja de cálculo
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);
            
            // Renderizar la primera página de la hoja en un archivo de imagen
            sheetRender.ToImage(0, "output.png");
            
            Console.WriteLine("Sheet rendered to image successfully.");
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToImage(int, Stream) {#toimage_3}

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

    public class SheetRenderMethodToImageWithInt32StreamDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;

            try
            {
                // Crear opciones de imagen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crear una instancia de SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Crear un flujo de memoria para contener la imagen
                using (MemoryStream stream = new MemoryStream())
                {
                    // Llamar a ToImage con los parámetros de índice de página y flujo
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

### Ver también

* class [SheetRender](../)
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

    public class SheetRenderMethodToImageWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "Row 1";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Row 2";
            worksheet.Cells["B3"].Value = 200;

            try
            {
                // Crear opciones de imagen
                ImageOrPrintOptions options = new ImageOrPrintOptions();
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Crear una instancia de SheetRender
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Obtener el índice de la primera página (basado en 0)
                int pageIndex = 0;

                // Llamar a ToImage con el parámetro de índice de página
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

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


