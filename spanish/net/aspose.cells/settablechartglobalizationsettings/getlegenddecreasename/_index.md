---
title: "SettableChartGlobalizationSettings.GetLegendDecreaseName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre de Disminución para la leyenda"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getlegenddecreasename/
---
## SettableChartGlobalizationSettings.GetLegendDecreaseName method

Obtiene el nombre de disminución para la leyenda

```csharp
public override string GetLegendDecreaseName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendDecreaseNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos simples para contexto (opcional)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Crear un gráfico (opcional, solo para tener un libro de trabajo completo)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Instanciar el objeto de configuración de globalización
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establecer una etiqueta personalizada de disminución de la leyenda
                settings.SetLegendDecreaseName("Custom Decrease Label");

                // Recuperar la etiqueta usando GetLegendDecreaseName
                string legendDecreaseName = settings.GetLegendDecreaseName();

                Console.WriteLine("Legend Decrease Name: " + legendDecreaseName);

                // Guardar el libro de trabajo (la configuración no está directamente adjunta al gráfico en esta demostración)
                workbook.Save("GetLegendDecreaseNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLegendDecreaseName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


