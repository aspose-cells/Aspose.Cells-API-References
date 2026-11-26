---
title: "Shape.ControlData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene los datos del control"
type: docs
url: /es/net/aspose.cells.drawing/shape/controldata/
---
## Shape.ControlData property

Obtiene los datos del control.

```csharp
public byte[] ControlData { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyControlDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma con los parámetros correctos
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Acceder a ControlData (propiedad de solo lectura)
            byte[] controlData = shape.ControlData;

            // Verificar ControlData
            if (controlData != null)
            {
                Console.WriteLine("ControlData exists with length: " + controlData.Length);
            }
            else
            {
                Console.WriteLine("No data.");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


