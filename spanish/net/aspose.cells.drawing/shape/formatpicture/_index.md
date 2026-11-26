---
title: "Shape.FormatPicture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece las opciones del formato de imagen"
type: docs
url: /es/net/aspose.cells.drawing/shape/formatpicture/
---
## Shape.FormatPicture property

Obtiene y establece las opciones del formato de imagen.

```csharp
public MsoFormatPicture FormatPicture { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyFormatPictureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una imagen a la hoja de cálculo
            int index = worksheet.Pictures.Add(0, 0, "example.jpg");
            Picture picture = worksheet.Pictures[index];
            
            // Acceder a la propiedad FormatPicture de la forma
            MsoFormatPicture msoFormatPicture = picture.FormatPicture;
            
            // Modificar las propiedades del formato de imagen
            msoFormatPicture.Brightness = 0.5f;
            msoFormatPicture.Contrast = 0.7f;
            msoFormatPicture.Transparency = 0.3f;
            
            // Guarda el libro de trabajo
            workbook.Save("ShapePropertyFormatPictureDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [MsoFormatPicture](../../msoformatpicture/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


