---
title: "Cells.HideColumns"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Ocultar varias columnas"
type: docs
url: /es/net/aspose.cells/cells/hidecolumns/
---
## Cells.HideColumns method

Oculta varias columnas.

```csharp
public void HideColumns(int column, int totalColumns)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| columna | Int32 | Índice de columna. |
| totalColumns | Int32 | Número de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodHideColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Ocultar columnas 3 a 5 (índice basado en cero)
            int startColumn = 2; // Column C
            int columnCount = 3;  // Hide 3 columns
            cells.HideColumns(startColumn, columnCount);

            // Guarda el libro de trabajo
            workbook.Save("HideColumnsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


