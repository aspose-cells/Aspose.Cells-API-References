---
title: "ShapeCollection.CopyInRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Copia las formas en el rango al rango de destino"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Copia las formas del rango al rango de destino.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Formas de origen. |
| ca | CellArea | El rango de origen. |
| destRow | Int32 | El índice de fila de destino del rango de destino. |
| destColumn | Int32 | La columna de destino del rango de destino. |
| isContained | Booleano | Indica si solo copiar las formas que están contenidas en el rango. Si es verdadero, solo copia las formas en el rango. De lo contrario, funciona como MS Office. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar una forma rectangular
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Define el área de celdas de la cual copiar
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Copiar formas dentro del rango especificado
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Guarda el libro de trabajo
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


