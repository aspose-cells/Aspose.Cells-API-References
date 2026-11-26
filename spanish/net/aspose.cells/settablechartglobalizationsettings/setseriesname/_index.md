---
title: "SettableChartGlobalizationSettings.SetSeriesName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el nombre de la Serie en el Gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setseriesname/
---
## SettableChartGlobalizationSettings.SetSeriesName method

Establece el nombre de la serie en el gráfico

```csharp
public void SetSeriesName(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | nombre dependiente local |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodSetSeriesNameWithStringDemo
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

                // Establecer un nombre personalizado de serie usando SetSeriesName con un parámetro de cadena
                settings.SetSeriesName("Custom Series Label");

                // Verificar la configuración obteniendo el nombre de la serie
                string seriesName = settings.GetSeriesName();
                Console.WriteLine($"Series name set to: {seriesName}");

                // Guarda el libro de trabajo
                workbook.Save("SetSeriesNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetSeriesName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


