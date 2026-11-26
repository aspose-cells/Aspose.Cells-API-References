---
title: "SettableChartGlobalizationSettings.SetChartTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el nombre del Título del Gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setcharttitlename/
---
## SettableChartGlobalizationSettings.SetChartTitleName method

Establece el nombre del título del gráfico

```csharp
public void SetChartTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetChartTitleNameDemo
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

                // Llamar a SetChartTitleName con una cadena personalizada
                settings.SetChartTitleName("Custom Chart Title");

                // Verifique la configuración obteniendo el valor
                string chartTitleName = settings.GetChartTitleName();
                Console.WriteLine("Chart Title Name set to: " + chartTitleName);

                // Guarda el libro de trabajo
                workbook.Save("SetChartTitleNameDemo.xlsx");
                Console.WriteLine("SetChartTitleName method called successfully. Workbook saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


