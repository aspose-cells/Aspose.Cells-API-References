---
title: "PivotArea.AxisType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Obtiene y establece la región de la tabla dinámica a la que se aplica esta regla"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/axistype/
---
## PivotArea.AxisType property

Obtiene y establece la región de la PivotTable a la que se aplica esta regla.

```csharp
public PivotFieldType AxisType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyAxisTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Electronics";
            worksheet.Cells["A3"].Value = "Clothing";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 800;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregue campos a áreas pivot
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);  // Sales

            // Crear y configurar PivotArea
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row; // Demonstrate AxisType property
            pivotArea.RuleType = PivotAreaType.Normal;

            // Seleccionar el área dinámica
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaAxisTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


