---
title: "Cells.IsRowHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Cells. Verifica si una fila en el índice dado está oculta"
type: docs
url: /es/net/aspose.cells/cells/isrowhidden/
---
## Cells.IsRowHidden method

Comprueba si una fila en el índice dado está oculta.

```csharp
public bool IsRowHidden(int rowIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowIndex | Int32 | índice de fila |

### Valor de retorno

verdadero si la fila está oculta

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsRowHiddenWithInt32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Datos de ejemplo
            cells[1, 0].PutValue("US");
            cells[2, 0].PutValue("UK");
            cells[3, 0].PutValue("India");
            cells[4, 0].PutValue("UK");
            cells[5, 0].PutValue("India");
            cells[6, 0].PutValue("US");
            
            // Aplicar filtro
            AutoFilter af = sheet.AutoFilter;
            af.Range = "A1:A1";
            af.Filter(0, "India");
            af.Refresh();
            
            // Verificar visibilidad de la fila
            Console.WriteLine("Row Visibility Check:");
            for (int i = 1; i < 7; i++)
            {
                Console.WriteLine($"Row {i} hidden: {cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


