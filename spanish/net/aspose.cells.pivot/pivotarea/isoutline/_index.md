---
title: "PivotArea.IsOutline"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Indica si la regla se refiere a un área que está en modo esquema"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/isoutline/
---
## PivotArea.IsOutline property

Indica si la regla se refiere a un área que está en modo de esquema.

```csharp
public bool IsOutline { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsOutlineDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Crear y configurar PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsOutline = false; // Disable outline style
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.DataAndLabel);

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaIsOutlineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


