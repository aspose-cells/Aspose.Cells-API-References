---
title: "Shape.RemoveHyperlink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Elimina el hipervínculo de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/removehyperlink/
---
## Shape.RemoveHyperlink method

Elimina el hipervínculo de la forma.

```csharp
public void RemoveHyperlink()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodRemoveHyperlinkDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma y establecer el hipervínculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 50, 50);
            shape.AddHyperlink("https://www.aspose.com");

            // Eliminar el hipervínculo
            shape.RemoveHyperlink();

            // Verificar que el hipervínculo se haya eliminado
            Console.WriteLine("Hyperlink removed: " + (shape.Hyperlink == null));

            // Guarda el libro de trabajo
            workbook.Save("ShapeRemoveHyperlinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


