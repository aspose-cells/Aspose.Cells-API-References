---
title: "Column.IsCollapsed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Column. Indica si la columna está colapsada"
type: docs
url: /es/net/aspose.cells/column/iscollapsed/
---
## Column.IsCollapsed property

si la columna está colapsada

```csharp
public bool IsCollapsed { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ColumnPropertyIsCollapsedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear y aplicar un estilo simple a la columna
            Style style = workbook.CreateStyle();
            style.BackgroundColor = Color.LightGray;
            
            Column column = worksheet.Cells.Columns[0];
            column.ApplyStyle(style, new StyleFlag { All = true });

            // Establecer propiedades de la columna incluyendo IsCollapsed
            column.Width = 15;
            column.IsCollapsed = true; // Demonstrating IsCollapsed property
            column.IsHidden = false;

            // Agregar algunos datos para visualizar la columna colapsada
            worksheet.Cells["A1"].PutValue("Collapsed Column");
            worksheet.Cells["B1"].PutValue("Visible Column");

            workbook.Save("ColumnIsCollapsedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


