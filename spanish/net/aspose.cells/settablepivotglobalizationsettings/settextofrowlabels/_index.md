---
title: "SettablePivotGlobalizationSettings.SetTextOfRowLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta Row Labels en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofrowlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfRowLabels method

Establece el texto de la etiqueta "Row Labels" en la tabla dinámica.

```csharp
public void SetTextOfRowLabels(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto de las etiquetas de fila |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfRowLabelsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el contexto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Crear configuraciones de globalización
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
            SettablePivotGlobalizationSettings pivotSettings = new SettablePivotGlobalizationSettings();
            globalizationSettings.PivotSettings = pivotSettings;

            try
            {
                // Establecer texto personalizado para "Row Labels"
                pivotSettings.SetTextOfRowLabels("Custom Row Labels");

                // Verificar el cambio
                string rowLabelsText = pivotSettings.GetTextOfRowLabels();
                Console.WriteLine($"Row Labels text after change: {rowLabelsText}");

                // Aplicar configuraciones al libro de trabajo
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Guarda el libro de trabajo
                workbook.Save("SetTextOfRowLabelsDemo.xlsx");
                Console.WriteLine("SetTextOfRowLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


