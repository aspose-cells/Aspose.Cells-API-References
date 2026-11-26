---
title: "Cells.DeleteRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento"
type: docs
url: /es/net/aspose.cells/cells/deleterange/
---
## Cells.DeleteRange method

Elimina un rango de celdas y desplaza las celdas según la opción de desplazamiento.

```csharp
public void DeleteRange(int startRow, int startColumn, int endRow, int endColumn, 
    ShiftType shiftType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | Índice de fila inicial. |
| startColumn | Int32 | Índice de columna inicial. |
| endRow | Int32 | Índice de fila final. |
| endColumn | Int32 | Índice de columna final. |
| shiftType | ShiftType | Opción de desplazar celdas. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRangeWithInt32Int32Int32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Poblar algunos datos de muestra
            sheet.Cells["A1"].PutValue("A1");
            sheet.Cells["B1"].PutValue("B1");
            sheet.Cells["C1"].PutValue("C1");
            sheet.Cells["A2"].PutValue("A2");
            sheet.Cells["B2"].PutValue("B2");
            sheet.Cells["C2"].PutValue("C2");

            // Eliminar rango y desplazar a la izquierda
            sheet.Cells.DeleteRange(0, 1, 1, 2, ShiftType.Left);

            // Guarda el libro de trabajo
            workbook.Save("DeleteRangeExample.xlsx");
        }
    }
}
```

### Ver también

* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


