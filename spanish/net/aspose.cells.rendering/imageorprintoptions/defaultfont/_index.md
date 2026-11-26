---
title: "ImageOrPrintOptions.DefaultFont"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Cuando los caracteres en el Excel son Unicode y no se establece la fuente correcta en el estilo de celda, pueden aparecer como bloques en pdfimage. Establezca la DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells utilizará la fuente predeterminada del sistema para mostrar estos caracteres Unicode."
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/defaultfont/
---
## ImageOrPrintOptions.DefaultFont property

Cuando los caracteres en el Excel son Unicode y no se establece una fuente correcta en el estilo de celda, pueden aparecer como bloques en pdf, imagen. Establezca la propiedad DefaultFont, como MingLiu o MS Gothic, para mostrar estos caracteres. Si esta propiedad no se establece, Aspose.Cells usará la fuente predeterminada del sistema para mostrar estos caracteres Unicode.

```csharp
public string DefaultFont { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyDefaultFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar texto de muestra a la celda
            worksheet.Cells["A1"].PutValue("Sample Text with Default Font");

            // Cree opciones de imagen y establezca la fuente predeterminada
            ImageOrPrintOptions imgOptions = new ImageOrPrintOptions
            {
                DefaultFont = "Arial", // Setting default font
                ImageType = ImageType.Png
            };

            // Renderiza la hoja de cálculo a una imagen
            SheetRender sheetRender = new SheetRender(worksheet, imgOptions);
            sheetRender.ToImage(0, "output.png");

            Console.WriteLine("Image generated with default font setting.");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


