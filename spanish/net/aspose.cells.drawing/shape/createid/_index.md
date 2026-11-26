---
title: "Shape.CreateId"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el ID de creación para esta forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Obtiene y establece el id de creación para esta forma.

```csharp
public Guid CreateId { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar una forma rectangular
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Crear y asignar un nuevo GUID como CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Guarda el libro de trabajo
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Recargar el libro de trabajo para verificar que el CreateId persista
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Mostrar el CreateId para verificación
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


