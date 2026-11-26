---
title: "PivotFilter.EvaluationOrder"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Obtiene el Orden de Evaluación del filtro pivot"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

Obtiene el orden de evaluación del filtro dinámico.

```csharp
public int EvaluationOrder { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Rellene datos de ejemplo
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Crear tabla dinámica
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // Agregar campos
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Agregar filtro pivot
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // Establecer propiedades del filtro incluyendo EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Actualizar tabla dinámica
            pivot.RefreshData();
            pivot.CalculateData();

            // Guardar el libro de trabajo
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


