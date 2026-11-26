---
title: "FillFormat.PictureFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene y establece el tipo de formato de imagen"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/pictureformattype/
---
## FillFormat.PictureFormatType property

Obtiene y establece el tipo de formato de imagen.

```csharp
public FillPictureType PictureFormatType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPictureFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar el relleno de imagen
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 1, 100, 200);

            // Establecer propiedades de relleno de imagen
            shape.Fill.Type = FillType.Texture;
            shape.Fill.Texture = TextureType.BlueTissuePaper;
            shape.Fill.PictureFormatType = FillPictureType.Stretch;

            // Guarda el libro de trabajo
            workbook.Save("FillFormatPictureTypeDemo.xlsx");

            // Cargue el libro de trabajo guardado para verificar las propiedades
            Workbook verifyWorkbook = new Workbook("FillFormatPictureTypeDemo.xlsx");
            Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];

            // Mostrar el PictureFormatType para demostrar su uso
            Console.WriteLine("PictureFormatType: " + verifyShape.Fill.PictureFormatType);
        }
    }
}
```

### Ver también

* enum [FillPictureType](../../fillpicturetype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


