---
title: "ImageOrPrintOptions.OnlyArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Si esta propiedad es true, se generará una sola Área y no se aplicará escala"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/onlyarea/
---
## ImageOrPrintOptions.OnlyArea property

Si esta propiedad es verdadera, se generará una Área y no se aplicará escala.

```csharp
public bool OnlyArea { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnlyAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Establecer opciones de imagen con la propiedad OnlyArea
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnlyArea = true; // Only render the used area

            // Renderiza la hoja de cálculo a una imagen
            SheetRender sr = new SheetRender(worksheet, options);
            using (MemoryStream ms = new MemoryStream())
            {
                sr.ToImage(0, ms);
                Console.WriteLine("Worksheet rendered to image with OnlyArea=true");
            }
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


