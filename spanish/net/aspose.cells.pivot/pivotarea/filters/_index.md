---
title: "PivotArea.Filters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Obtiene todos los filtros para este área de pivote"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/filters/
---
## PivotArea.Filters property

Obtiene todos los filtros para esta PivotArea.

```csharp
public PivotAreaFilterCollection Filters { get; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyFiltersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "SalesData";
            
            // Crear datos de ejemplo
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Revenue");
            dataSheet.Cells["A2"].PutValue("Electronics");
            dataSheet.Cells["B2"].PutValue(1500);
            dataSheet.Cells["A3"].PutValue("Furniture");
            dataSheet.Cells["B3"].PutValue(800);
            dataSheet.Cells["A4"].PutValue("Electronics");
            dataSheet.Cells["B4"].PutValue(2200);

            // Crear tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Configurar campo de fila con subtotales
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;

            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");

            // Crear área de pivote y seleccionar campos
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
            pivotArea.SelectField(PivotFieldType.Row, "Category");

            // Demostrar el uso de la propiedad Filters
            Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
            if (pivotArea.Filters.Count > 1)
            {
                bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
                Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
            }

            workbook.Save("PivotFiltersDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


