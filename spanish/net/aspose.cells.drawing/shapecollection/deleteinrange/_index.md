---
title: "ShapeCollection.DeleteInRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Elimina formas en el rango. Las formas de comentario no serán eliminadas."
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Elimina las formas en el rango. Las formas de comentario no se eliminarán.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El rango. Si las formas están contenidas en el rango, serán eliminadas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar primera forma rectangular
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Agregar segunda forma rectangular
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Definir el rango donde se deben eliminar las formas
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Eliminar formas dentro del rango especificado
            shapes.DeleteInRange(area);

            // Guardar el libro de trabajo (opcional)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


