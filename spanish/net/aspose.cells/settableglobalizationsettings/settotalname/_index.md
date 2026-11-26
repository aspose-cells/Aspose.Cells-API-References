---
title: "SettableGlobalizationSettings.SetTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre total de una función específica"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/settotalname/
---
## SettableGlobalizationSettings.SetTotalName method

Establece el nombre total de la función específica.

```csharp
public void SetTotalName(ConsolidationFunction functionType, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | ConsolidationFunction | El tipo de función. |
| name | String | El nombre total de la función. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para la consolidación
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["A4"].PutValue("Total");

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Establecer un nombre total personalizado para la función Sum
                settings.SetTotalName(ConsolidationFunction.Sum, "Custom Sum Total");
                
                // Establecer nombre total personalizado para la función Average
                settings.SetTotalName(ConsolidationFunction.Average, "Custom Average Total");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                // Verificar la configuración obteniendo los valores de nuevo
                string sumTotalName = settings.GetTotalName(ConsolidationFunction.Sum);
                string avgTotalName = settings.GetTotalName(ConsolidationFunction.Average);

                Console.WriteLine($"Sum total name set to: {sumTotalName}");
                Console.WriteLine($"Average total name set to: {avgTotalName}");

                // Crear una tabla dinámica para demostrar el efecto
                worksheet.Cells["D1"].PutValue("Pivot Table");
                var pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
                var pivotTable = worksheet.PivotTables[pivotIndex];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                // Guarda el libro de trabajo
                workbook.Save("SetTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTotalName method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


