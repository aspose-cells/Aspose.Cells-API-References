---
title: "Row.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Indica si la fila está oculta"
type: docs
url: /es/net/aspose.cells/row/ishidden/
---
## Row.IsHidden property

Indica si la fila está oculta.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            for (int i = 0; i < 10; i++)
            {
                cells[$"A{i + 1}"].PutValue($"Row {i + 1}");
            }

            // Ocultar algunas filas
            cells.HideRow(2);  // Row 3 (0-based index 2)
            cells.HideRow(5);  // Row 6 (0-based index 5)
            cells.HideRow(8);  // Row 9 (0-based index 8)

            // Comprobar y mostrar el estado IsHidden de cada fila
            for (int i = 0; i < 10; i++)
            {
                bool isHidden = cells.Rows[i].IsHidden;
                Console.WriteLine($"Row {i + 1} is hidden: {isHidden}");
            }

            // Guarda el libro de trabajo
            workbook.Save("RowHiddenDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


