---
title: "Shape.Spid"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Especifica un identificador de cadena opcional que una aplicación puede usar para identificar la forma particular"
type: docs
url: /es/net/aspose.cells.drawing/shape/spid/
---
## Shape.Spid property

Especifica un identificador de cadena opcional que una aplicación puede usar para identificar la forma particular.

```csharp
public string Spid { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySpidDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular a la hoja de cálculo con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 150, 0);

            // Obtener y mostrar la propiedad Spid de la forma
            string spid = shape.Spid;
            Console.WriteLine("Shape SPID: " + spid);

            // Guarda el libro de trabajo
            workbook.Save("ShapePropertySpidDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


