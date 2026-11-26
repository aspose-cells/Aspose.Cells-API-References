---
title: "Cells.HideGroupDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Contrae las filas/columnas agrupadas"
type: docs
url: /es/net/aspose.cells/cells/hidegroupdetail/
---
## Cells.HideGroupDetail method

Contrae las filas/columnas agrupadas.

```csharp
public void HideGroupDetail(bool isVertical, int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isVertical | Booleano | Verdadero, contrae las filas agrupadas. |
| índice | Int32 | El índice de fila/columna |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideGroupDetailWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrupa filas y oculta los detalles
            worksheet.Cells.GroupRows(0, 9, false);
            worksheet.Cells.HideGroupDetail(true, 4);
            worksheet.Cells.HideGroupDetail(true, 7);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


