---
title: "ShapePath.ShapePath"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor ShapePath. Inicializa una nueva instancia de la clase ShapePath"
type: docs
url: /es/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Inicializa una nueva instancia de la clase [`ShapePath`](../).

```csharp
public ShapePath()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Cree una nueva ruta de forma utilizando el método #ctor
                ShapePath shapePath = new ShapePath();

                // Añada segmentos de ruta para crear una forma simple
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //agregar forma libre
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


