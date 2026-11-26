---
title: "FillFormat.Transparency"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FillFormat. Devuelve o establece el grado de transparencia del área como un valor de 0.0 opaco a 1.0 transparente"
type: docs
url: /es/net/aspose.cells.drawing/fillformat/transparency/
---
## FillFormat.Transparency property

Devuelve o establece el grado de transparencia del área como un valor de 0.0 (opaco) a 1.0 (claro).

```csharp
public double Transparency { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma para demostrar la transparencia
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 200, 100, 50, 50);

            // Establecer propiedades de relleno con transparencia
            shape.Fill.FillType = FillType.Solid;
            shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            shape.Fill.Transparency = 0.3; // 30% transparent

            // Guarda el libro de trabajo
            workbook.Save("FillFormatTransparencyDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


