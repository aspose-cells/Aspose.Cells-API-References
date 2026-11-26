---
title: "SettableGlobalizationSettings.SetGrandTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre del total general de una función específica"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setgrandtotalname/
---
## SettableGlobalizationSettings.SetGrandTotalName method

Establece el nombre del total general de la función específica.

```csharp
public void SetGrandTotalName(ConsolidationFunction functionType, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| functionType | ConsolidationFunction | El tipo de función. |
| name | String | El nombre del total general de la función. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettableGlobalizationSettingsMethodSetGrandTotalNameWithConsolidationFunctionStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruit");
            worksheet.Cells["A3"].PutValue("Fruit");
            worksheet.Cells["A4"].PutValue("Vegetable");
            worksheet.Cells["B1"].PutValue("Amount");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(75);

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llamar a SetGrandTotalName con ConsolidationFunction.Sum y nombre personalizado
                settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Grand Total");

                // Actualizar la tabla dinámica para aplicar los cambios
                pivotTable.RefreshData();
                pivotTable.CalculateData();

                Console.WriteLine("Grand total name set to 'Custom Grand Total' for Sum function");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGrandTotalName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("MethodSetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


