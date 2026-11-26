---
title: "PivotField.Function"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Representa la función utilizada para resumir este campo de datos de PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Representa la función utilizada para resumir este campo de datos de tabla dinámica.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyFunctionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 120;
            cells["A4"].Value = "A";
            cells["B4"].Value = 80;
            cells["A5"].Value = "B";
            cells["B5"].Value = 60;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Agregar campo de datos y establecer la función a Max
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[fieldIndex];
            dataField.Function = ConsolidationFunction.Max;

            // Calcular tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotFieldFunctionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


