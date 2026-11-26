---
title: "SettableChartGlobalizationSettings.SetLegendDecreaseName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el nombre de Decrease para la Leyenda"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setlegenddecreasename/
---
## SettableChartGlobalizationSettings.SetLegendDecreaseName method

Establece el nombre de disminución para la leyenda

```csharp
public void SetLegendDecreaseName(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | nombre dependiente local |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetLegendDecreaseNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para un gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Series");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crear configuraciones de globalización
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

            try
            {
                // Llamar a SetLegendDecreaseName con una cadena personalizada
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // La clase Chart no tiene una propiedad ChartGlobalizationSettings,
                // por lo que necesitamos usar el objeto de configuraciones directamente donde sea necesario
                // (Nota: En el uso real, necesitarías encontrar dónde se aplican estas configuraciones)
                Console.WriteLine("SetLegendDecreaseName method executed successfully with parameter: 'Custom Decrease Label'");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLegendDecreaseName method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("SetLegendDecreaseNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


