---
title: "Shape.RemoveActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de Shape. Eliminar control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing/shape/removeactivexcontrol/
---
## Shape.RemoveActiveXControl method

Elimina el control ActiveX.

```csharp
public void RemoveActiveXControl()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveActiveXControlDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma que contendrá el control ActiveX
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.CommandButton, 
                1, 1, 1, 1, 100, 50);
            
            // Eliminar el control ActiveX si existe
            if (shape.ActiveXControl != null)
            {
                shape.RemoveActiveXControl();
                Console.WriteLine("ActiveX control removed successfully.");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


