---
title: "ImageOrPrintOptions.PageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Obtiene o establece el número de páginas a guardar"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Obtiene o establece el número de páginas a guardar.

```csharp
public int PageCount { get; set; }
```

### Observaciones

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Page 1 Data");
            worksheet.Cells["A2"].PutValue("Sample Content");
            worksheet.Cells["A3"].PutValue("Demo for PageCount");
            
            // Establecer el área de impresión y la configuración de página
            worksheet.PageSetup.PrintArea = "A1:A3";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
            options.OnlyArea = true;

            // Renderiza la hoja de cálculo a una imagen
            SheetRender renderer = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Guarda la imagen en un archivo
                string outputPath = "output.png";
                File.WriteAllBytes(outputPath, stream.ToArray());
                Console.WriteLine($"Output saved to: {outputPath}");
            }
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


