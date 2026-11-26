---
title: "Shape.MacroName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene y establece el nombre de la macro"
type: docs
url: /es/net/aspose.cells.drawing/shape/macroname/
---
## Shape.MacroName property

Obtiene y establece el nombre de la macro.

```csharp
public string MacroName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyMacroNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Establecer el nombre de la macro para la forma
            shape.MacroName = "DoWork()";

            // Confirmación de salida
            Console.WriteLine("Shape macro name set to: " + shape.MacroName);
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


