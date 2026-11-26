---
title: "SettablePivotGlobalizationSettings.SetTextOfAll"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta All en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofall/
---
## SettablePivotGlobalizationSettings.SetTextOfAll method

Establece el texto de la etiqueta "(All)" en la tabla dinámica.

```csharp
public void SetTextOfAll(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | texto personalizado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfAllWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Crear tabla dinámica
            var pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crear configuraciones de globalización
            var settings = new SettableGlobalizationSettings();
            settings.PivotSettings = new SettablePivotGlobalizationSettings();

            try
            {
                // Llamar al método SetTextOfAll para cambiar el texto "(All)"
                ((SettablePivotGlobalizationSettings)settings.PivotSettings).SetTextOfAll("All Products");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;
                pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium2;

                Console.WriteLine("SetTextOfAll method executed successfully. Changed '(All)' to 'All Products'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTextOfAll method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SettablePivotGlobalizationSettingsMethodSetTextOfAllDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


