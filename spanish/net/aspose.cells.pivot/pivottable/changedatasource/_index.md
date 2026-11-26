---
title: "PivotTable.ChangeDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Cambiar la fuente de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/changedatasource/
---
## PivotTable.ChangeDataSource method

Cambia el origen de datos de la tabla dinámica.

```csharp
public void ChangeDataSource(string[] source)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class PivotTableMethodChangeDataSourceWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crear una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Preparar nueva fuente de datos
            string[] newDataSource = new string[] { "C1:D4", "Sheet1" };

            try
            {
                // Cambiar la fuente de datos de la tabla dinámica
                pivotTable.ChangeDataSource(newDataSource);

                // Actualizar la tabla dinámica para aplicar los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable data source changed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing pivot table data source: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("PivotTableChangeDataSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


