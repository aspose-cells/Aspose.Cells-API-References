---
title: "FillFormat.FillType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Obtiene y establece el tipo de relleno"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/filltype/
---
## FillFormat.FillType property

Obtiene y establece el tipo de relleno

```csharp
public FillType FillType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Establezca un relleno sólido con color
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Red;

            // Muestre el tipo de relleno
            Console.WriteLine("Shape fill type: " + shape.Fill.FillType);

            // Cambie a relleno degradado
            shape.Fill.FillType = FillType.Gradient;
            Console.WriteLine("Shape fill type changed to: " + shape.Fill.FillType);

            // Guarda el libro de trabajo
            workbook.Save("FillTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FillType](../../filltype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


