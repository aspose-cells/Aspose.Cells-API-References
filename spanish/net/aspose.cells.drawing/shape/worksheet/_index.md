---
title: "Shape.Worksheet"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene el objeto Worksheet que contiene esta forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/worksheet/
---
## Shape.Worksheet property

Obtiene el objeto [`Worksheet`](../../../aspose.cells/worksheet/) que contiene esta forma.

```csharp
public Worksheet Worksheet { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            
            // Demostrar el uso de la propiedad Worksheet
            Worksheet shapeWorksheet = shape.Worksheet;
            
            // Muestre el nombre del Worksheet para demostrar que la propiedad funciona
            Console.WriteLine("Shape belongs to worksheet: " + shapeWorksheet.Name);
        }
    }
}
```

### Ver también

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


