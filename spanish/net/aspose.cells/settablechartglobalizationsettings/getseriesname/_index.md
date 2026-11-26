---
title: "SettableChartGlobalizationSettings.GetSeriesName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre de Series en el Gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getseriesname/
---
## SettableChartGlobalizationSettings.GetSeriesName method

Obtiene el nombre de la serie en el gráfico

```csharp
public override string GetSeriesName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetSeriesNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Column A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C1"].PutValue("Column B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Crear y aplicar configuraciones de globalización
            SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();
            settings.SetSeriesName("Custom Series Name");
            
            // Las configuraciones de globalización se utilizan al renderizar/mostrar el gráfico,
            // pero no se asignan directamente al objeto gráfico
            // (ya que la clase Chart no tiene esta propiedad)

            try
            {
                // Obtener el nombre de serie personalizado
                string seriesName = settings.GetSeriesName();
                Console.WriteLine("Series Name: " + seriesName);

                // Guarda el libro de trabajo
                workbook.Save("MethodGetSeriesNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetSeriesName method: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


