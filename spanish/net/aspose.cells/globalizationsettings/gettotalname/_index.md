---
title: "GlobalizationSettings.GetTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre total de la función"
type: docs
url: /es/net/aspose.cells/globalizationsettings/gettotalname/
---
## GlobalizationSettings.GetTotalName method

Obtiene el nombre total de la función.

```csharp
public virtual string GetTotalName(ConsolidationFunction functionType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | ConsolidationFunction | El tipo de función. |

### Valor de retorno

El nombre total de la función.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class GlobalizationSettingsMethodGetTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B3"].Value = 2500;
            worksheet.Cells["A4"].Value = "Bike";
            worksheet.Cells["B4"].Value = 1500;

            // Cree configuraciones de globalización personalizadas
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demostrar llamada directa al método
                Console.WriteLine("Sum Total Name: " + 
                    customSettings.GetTotalName(ConsolidationFunction.Sum));
                
                // Crear tabla dinámica para activar el uso de GetTotalName
                int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "D1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                PivotField dataField = pivotTable.DataFields[dataFieldIndex];
                dataField.Function = ConsolidationFunction.Sum;

                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("PivotTable created with custom total names");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsMethodGetTotalNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTotalName(ConsolidationFunction functionType)
            {
                return functionType switch
                {
                    ConsolidationFunction.Sum => "[Sum Custom]",
                    ConsolidationFunction.Count => "[Count Custom]",
                    _ => base.GetTotalName(functionType)
                };
            }
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


