---
title: "Row.IsCollapsed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Row. Indica si la fila está colapsada"
type: docs
url: /es/net/aspose.cells/row/iscollapsed/
---
## Row.IsCollapsed property

si la fila está colapsada

```csharp
public bool IsCollapsed { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear y dar estilo a una fila
            Row row = worksheet.Cells.Rows[0];
            row.Height = 20;
            row.GroupLevel = 1;
            
            // Demostrar la propiedad IsCollapsed
            row.IsCollapsed = true;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Expandir la fila
            row.IsCollapsed = false;
            Console.WriteLine("Row is collapsed: " + row.IsCollapsed);

            // Guarda el libro de trabajo
            workbook.Save("RowIsCollapsedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


