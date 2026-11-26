---
title: "PivotField.ClearFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotField. Elimina la configuración de filtro en este campo dinámico"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/clearfilter/
---
## PivotField.ClearFilter method

Borra la configuración de filtro en este pivot field.

```csharp
public void ClearFilter()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotFieldMethodClearFilterDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["A4"].Value = "Fruit";
            worksheet.Cells["A5"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;
            worksheet.Cells["B5"].Value = 300;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campo de fila
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Agregar campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Obtener el campo de pivote
            PivotField pivotField = pivotTable.RowFields[0];

            try
            {
                // Aplica un filtro primero para demostrar cómo eliminarlo
                pivotField.FilterByLabel(PivotFilterType.CaptionEqual, "Fruit", null);

                // Llama al método ClearFilter
                pivotField.ClearFilter();

                Console.WriteLine("ClearFilter method executed successfully");
                Console.WriteLine("All filters have been removed from the pivot field");

                // Actualiza la tabla dinámica para mostrar los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFilter method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("PivotFieldMethodClearFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


