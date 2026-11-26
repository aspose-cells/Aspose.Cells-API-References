---
title: "MsoFormatPicture.IsGray"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoFormatPicture. Indica si esta imagen debe mostrarse en escala de grises"
type: docs
url: /es/net/aspose.cells.drawing/msoformatpicture/isgray/
---
## MsoFormatPicture.IsGray property

Indica si esta imagen debe mostrarse en escala de grises.

```csharp
public bool IsGray { get; set; }
```

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFormatPicturePropertyIsGrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de imagen
            using (Stream imageStream = File.OpenRead("example.gif"))
            {
                Shape shape = worksheet.Shapes.AddPicture(0, 0, imageStream, 100, 100);
                
                // Establecer propiedades de formato de imagen
                shape.FormatPicture.Brightness = 90;
                shape.FormatPicture.Contrast = 90;
                shape.FormatPicture.IsGray = true;

                // Guarda el libro de trabajo
                workbook.Save("output.xlsx");
            }

            // Recargar y verificar las propiedades
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Brightness: " + loadedShape.FormatPicture.Brightness);
            Console.WriteLine("Contrast: " + loadedShape.FormatPicture.Contrast);
            Console.WriteLine("IsGray: " + loadedShape.FormatPicture.IsGray);
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


