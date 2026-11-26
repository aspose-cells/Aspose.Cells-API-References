---
title: "ShapeCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeCollection. Obtiene el objeto Shape en el índice específico de la lista"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/item/
---
## ShapeCollection indexer (1 of 2)

Obtiene el [`Shape`](../../shape/) objeto en el índice específico de la lista.

```csharp
public Shape this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añade algunas formas a la hoja de cálculo con los parámetros correctos
            worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            worksheet.Shapes.AddLine(3, 0, 300, 100, 100, 100);

            // Obtén la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Demostrar la propiedad Item obteniendo la primera forma
            Shape firstShape = shapes[0];
            Console.WriteLine("First shape type: " + firstShape.Type);

            // Demostrar la propiedad Item obteniendo la forma por ID
            Shape shapeById = shapes[2];
            Console.WriteLine("Shape with ID 2 type: " + shapeById.Type);
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## ShapeCollection indexer (2 of 2)

Obtiene el objeto [`Shape`](../../shape/) por el nombre de la forma.

```csharp
public Shape this[string name] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| name | El nombre de la forma. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar formas a la hoja de cálculo
            ShapeCollection shapes = worksheet.Shapes;
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);
            shapes.AddOval(5, 0, 2, 0, 130, 130);
            
            // Acceder a las formas usando la propiedad Item
            Shape rectangle = shapes["Rectangle 1"];
            if (rectangle != null)
            {
                rectangle.FillFormat.ForeColor = System.Drawing.Color.Red;
            }
            
            Shape oval = shapes["Oval 2"];
            if (oval != null)
            {
                oval.FillFormat.ForeColor = System.Drawing.Color.Blue;
            }
            
            // Guarda el libro de trabajo
            workbook.Save("ShapeCollectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


