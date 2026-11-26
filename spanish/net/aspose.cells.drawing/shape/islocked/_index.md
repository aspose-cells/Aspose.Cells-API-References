---
title: "Shape.IsLocked"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Verdadero significa que el objeto no puede modificarse cuando la hoja está protegida. Nota que este valor solo tiene sentido si la hoja de cálculo o los objetos en la hoja están protegidos"
type: docs
url: /es/net/aspose.cells.drawing/shape/islocked/
---
## Shape.IsLocked property

True indica que el objeto no puede modificarse cuando la hoja está protegida. Note que este valor solo tiene sentido si la hoja de cálculo o los objetos en la hoja están protegidos.

```csharp
public bool IsLocked { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 100);

            // Proteger la hoja de cálculo
            worksheet.Protect(ProtectionType.All);

            // Demostrar el bloqueo/desbloqueo de la forma
            Console.WriteLine("Original IsLocked state: " + shape.IsLocked);

            // Desbloquear la forma
            shape.IsLocked = false;
            Console.WriteLine("After unlocking, IsLocked state: " + shape.IsLocked);

            // Bloquear la forma
            shape.IsLocked = true;
            Console.WriteLine("After locking, IsLocked state: " + shape.IsLocked);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


