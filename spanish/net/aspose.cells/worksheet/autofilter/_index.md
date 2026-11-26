---
title: "Worksheet.AutoFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Worksheet. Representa el filtro automático para la hoja de cálculo especificada"
type: docs
url: /es/net/aspose.cells/worksheet/autofilter/
---
## Worksheet.AutoFilter property

Representa el filtro automático para la hoja de cálculo especificada.

```csharp
public AutoFilter AutoFilter { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Shirt");
            worksheet.Cells["B3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Phone");
            worksheet.Cells["B4"].PutValue("Electronics");
            worksheet.Cells["A5"].PutValue("Pants");
            worksheet.Cells["B5"].PutValue("Clothing");

            // Aplicar filtro automático
            worksheet.AutoFilter.Range = "A1:B5";
            worksheet.AutoFilter.Filter(1, "Electronics");

            // Actualizar el filtro
            worksheet.AutoFilter.Refresh();

            // Guarda el libro de trabajo
            workbook.Save("AutoFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [AutoFilter](../../autofilter/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


