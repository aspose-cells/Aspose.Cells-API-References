---
title: "Worksheet.SelectRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Worksheet. Selecciona un rango"
type: docs
url: /es/net/aspose.cells/worksheet/selectrange/
---
## Worksheet.SelectRange method

Selecciona un rango.

```csharp
public void SelectRange(int startRow, int startColumn, int totalRows, int totalColumns, 
    bool removeOthers)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startRow | Int32 | La fila de inicio. |
| startColumn | Int32 | La columna de inicio |
| totalRows | Int32 | El número de filas. |
| totalColumns | Int32 | El número de columnas |
| removeOthers | Booleano | True significa eliminar otras áreas seleccionadas y solo seleccionar este rango. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSelectRangeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Seleccionar rango desde la fila 1, columna 1 hasta la fila 5, columna 5 (B2:F6) y hacerlo activo
            worksheet.SelectRange(1, 1, 5, 5, true);
            
            Console.WriteLine("Active cell: " + worksheet.ActiveCell);
        }
    }
}
```

### Ver también

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


