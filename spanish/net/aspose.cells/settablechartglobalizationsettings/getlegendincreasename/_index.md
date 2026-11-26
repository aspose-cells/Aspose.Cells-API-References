---
title: "SettableChartGlobalizationSettings.GetLegendIncreaseName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre de aumento para la leyenda"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getlegendincreasename/
---
## SettableChartGlobalizationSettings.GetLegendIncreaseName method

Obtiene el nombre de aumento para la leyenda

```csharp
public override string GetLegendIncreaseName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendIncreaseNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos mínimos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establecer un nombre personalizado de aumento de la leyenda
                settings.SetLegendIncreaseName("Custom Increase Label");

                // Obtener el nombre de aumento de la leyenda usando GetLegendIncreaseName
                string legendIncreaseName = settings.GetLegendIncreaseName();
                Console.WriteLine("Legend Increase Name: " + legendIncreaseName);

                // Guarda el libro de trabajo
                workbook.Save("GetLegendIncreaseNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendIncreaseName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


