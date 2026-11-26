---
title: "Outline.SummaryRowBelow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Outline. Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema"
type: docs
url: /es/net/aspose.cells/outline/summaryrowbelow/
---
## Outline.SummaryRowBelow property

Indica si la fila de resumen se posicionará debajo de las filas de detalle en el esquema.

```csharp
public bool SummaryRowBelow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OutlinePropertySummaryRowBelowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y agrupación
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("Total");
            worksheet.Cells["B4"].PutValue("=SUM(B2:B3)");
            
            // Agrupar filas y establecer la posición de la fila de resumen
            worksheet.Cells.GroupRows(1, 2, false);
            Outline outline = worksheet.Outline;
            outline.SummaryRowBelow = true;
            
            workbook.Save("OutlineSummaryRowBelow.xlsx");
        }
    }
}
```

### Ver también

* class [Outline](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


