---
title: "Shape.IsLockAspectRatio"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. True indica que la proporción de aspecto de la forma está bloqueada"
type: docs
url: /es/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

True indica que la relación de aspecto de la forma está bloqueada.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### Observaciones

Solo para imágenes y objetos Ole. NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad Shape.IsAspectRatioLocked. Esta propiedad será eliminada 12 meses después, a partir de julio de 2024. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Bloquear proporción de aspecto
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // Desbloquear proporción de aspecto
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


