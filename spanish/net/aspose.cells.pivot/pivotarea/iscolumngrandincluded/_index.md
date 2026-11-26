---
title: "PivotArea.IsColumnGrandIncluded"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Indica si el total general de columna está incluido"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/iscolumngrandincluded/
---
## PivotArea.IsColumnGrandIncluded property

Indica si el total general de la columna está incluido.

```csharp
public bool IsColumnGrandIncluded { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsColumnGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurar el área de pivote
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.RuleType = PivotAreaType.Normal;

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


