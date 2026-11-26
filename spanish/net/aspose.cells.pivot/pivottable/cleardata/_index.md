---
title: "PivotTable.ClearData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Borrar datos y formato de la vista de PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/cleardata/
---
## PivotTable.ClearData method

Borra los datos y el formato de la vista de tabla dinámica.

```csharp
public void ClearData()
```

### Observaciones

Si este método no se llama antes de agregar o eliminar PivotField, es posible que los datos de la PivotTable no se corrijan

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodClearDataDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(15);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("Pivot table with data:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Borrar datos de la tabla dinámica
            pivotTable.ClearData();
            Console.WriteLine("\nAfter ClearData():");
            Console.WriteLine("Pivot table row count: " + (pivotTable.DataBodyRange.EndRow - pivotTable.DataBodyRange.StartRow + 1));

            // Reconstruir la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nRebuilt pivot table:");
            Console.WriteLine(worksheet.Cells["D1"].StringValue);
            Console.WriteLine(worksheet.Cells["D2"].StringValue);
            Console.WriteLine(worksheet.Cells["D3"].StringValue);

            // Guardar el libro de trabajo
            workbook.Save("PivotTableClearDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


