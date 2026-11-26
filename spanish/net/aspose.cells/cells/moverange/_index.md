---
title: "Cells.MoveRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Mueve el rango"
type: docs
url: /es/net/aspose.cells/cells/moverange/
---
## Cells.MoveRange method

Mueve el rango.

```csharp
public void MoveRange(CellArea sourceArea, int destRow, int destColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceArea | CellArea | El rango que debe moverse. |
| destRow | Int32 | La fila dest. |
| destColumn | Int32 | La columna dest. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMoveRangeWithCellAreaInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Colocar valores en celdas
            cells["A1"].PutValue("Original");
            cells["B1"].PutValue(100);
            cells["A2"].PutValue("Data");
            cells["B2"].PutValue(200);

            // Defina el área de celdas a mover (A1:B2)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 1;
            area.EndColumn = 1;

            // Mueva el rango hacia abajo 2 filas y a la derecha 3 columnas
            cells.MoveRange(area, 2, 3);

            // Guarda el libro de trabajo
            workbook.Save("MoveRangeExample.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


