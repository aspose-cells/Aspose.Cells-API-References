---
title: "SheetRender.ToTiff"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SheetRender. Renderiza toda la hoja de cálculo como imagen Tiff a un flujo"
type: docs
url: /es/net/aspose.cells.rendering/sheetrender/totiff/
---
## ToTiff(Stream) {#totiff}

Renderizar toda la hoja de cálculo como imagen Tiff a un flujo.

```csharp
public void ToTiff(Stream stream)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| stream | Stream | el flujo de la imagen de salida |

### Ejemplos

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
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue contenido de ejemplo para demostrar el renderizado
            worksheet.Cells["A1"].PutValue("Aspose.Cells TIFF Rendering Demo");
            
            // Configure opciones de imagen para el renderizado
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;

            // Cree el renderizador de hoja con opciones configuradas
            SheetRender renderer = new SheetRender(worksheet, options);
            try
            {
                // Cree un flujo de salida para la imagen TIFF
                using (FileStream tiffStream = new FileStream("output.tiff", FileMode.Create))
                {
                    // Renderice la hoja de cálculo a TIFF usando el flujo
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

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)

---

## ToTiff(string) {#totiff_1}

Renderizar toda la hoja de cálculo como imagen Tiff a un archivo.

```csharp
public void ToTiff(string filename)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre de archivo | String | el nombre de archivo de la imagen de salida |

### Ejemplos

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
            // Cargar el archivo Excel de origen
            Workbook workbook = new Workbook("Book1.xlsx");

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.SaveFormat = SaveFormat.Tiff;

            // Crear renderizado de hoja para la primera hoja de cálculo
            SheetRender sheetRender = new SheetRender(workbook.Worksheets[0], options);

            // Guarde todas las páginas de la hoja como un archivo TIFF multipágina
            sheetRender.ToTiff("output.tiff");
        }
    }
}
```

### Ver también

* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


