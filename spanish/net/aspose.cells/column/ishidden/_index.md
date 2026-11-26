---
title: "Column.IsHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Indica si la columna está oculta"
type: docs
url: /es/net/aspose.cells/column/ishidden/
---
## Column.IsHidden property

Indica si la columna está oculta.

```csharp
public bool IsHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer el ancho de la columna para la demostración
            worksheet.Cells.Columns[1].Width = 20;
            Console.WriteLine("Column 1 width before hiding: " + worksheet.Cells.Columns[1].Width);

            // Ocultar la columna
            worksheet.Cells.Columns[1].IsHidden = true;
            Console.WriteLine("Column 1 is hidden: " + worksheet.Cells.Columns[1].IsHidden);

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


