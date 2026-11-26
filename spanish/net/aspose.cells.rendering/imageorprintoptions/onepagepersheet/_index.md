---
title: "ImageOrPrintOptions.OnePagePerSheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ImageOrPrintOptions. Si OnePagePerSheet es true, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido y los demás ajustes de la configuración de página seguirán teniendo efecto"
type: docs
url: /es/net/aspose.cells.rendering/imageorprintoptions/onepagepersheet/
---
## ImageOrPrintOptions.OnePagePerSheet property

Si OnePagePerSheet es verdadero, todo el contenido de una hoja se exportará a una sola página en el resultado. El tamaño de papel de la configuración de página será inválido, y los demás ajustes de la configuración de página seguirán teniendo efecto.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Sample Data for OnePagePerSheet Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Row " + i);
            }

            // Crear opciones de imagen o impresión
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true; // Key property being demonstrated
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Crear renderizado de hoja
            SheetRender sr = new SheetRender(worksheet, options);
            
            // Guardar la imagen de salida
            sr.ToImage(0, "OnePagePerSheetOutput.png");
            
            Console.WriteLine("Output saved with OnePagePerSheet=true");
        }
    }
}
```

### Ver también

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


