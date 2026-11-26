---
title: "MsoLineFormat.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Indica si el objeto es visible"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Indica si el objeto es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma rectangular con borde visible
            var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape1.LineFormat.IsVisible = true;

            // Agregar una forma ovalada con borde invisible
            var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            shape2.LineFormat.IsVisible = false;

            // Verificar e imprimir los valores de la propiedad IsVisible
            Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
            Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);

            // Guarda el libro de trabajo
            workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


