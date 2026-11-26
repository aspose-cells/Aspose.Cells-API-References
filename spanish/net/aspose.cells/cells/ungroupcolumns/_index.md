---
title: "Cells.UngroupColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Desagrupa columnas"
type: docs
url: /es/net/aspose.cells/cells/ungroupcolumns/
---
## Cells.UngroupColumns method

Desagrupa columnas.

```csharp
public void UngroupColumns(int firstIndex, int lastIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstIndex | Int32 | El índice de la primera columna a desagrupar. |
| lastIndex | Int32 | El índice de la última columna a desagrupar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodUngroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrupar columnas primero para demostrar el desagrupamiento
            worksheet.Cells.GroupColumns(0, 2);

            // Desagrupar columnas (0 a 2)
            worksheet.Cells.UngroupColumns(0, 2);

            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


