---
title: "ImageOrPrintOptions.CheckWorkbookDefaultFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Cuando los caracteres en el Excel son Unicode y no se establecen con la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdfimage. Establezca esto en true para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/
---
## ImageOrPrintOptions.CheckWorkbookDefaultFont property

Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca esto en verdadero para intentar usar la fuente predeterminada del libro de trabajo y mostrar estos caracteres primero.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("Sample Text");
            
            // Establecer la fuente predeterminada para el libro de trabajo
            workbook.DefaultStyle.Font.Name = "Arial";
            workbook.DefaultStyle.Font.Size = 12;

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Habilitar la verificación de la fuente predeterminada del libro de trabajo
            options.CheckWorkbookDefaultFont = true;

            // Renderiza la hoja de cálculo a una imagen
            SheetRender renderer = new SheetRender(sheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Guarda la imagen en un archivo
                using (FileStream file = new FileStream("output.png", FileMode.Create))
                {
                    stream.WriteTo(file);
                }
            }
            
            Console.WriteLine("Image generated with workbook default font check.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


