---
title: "SettableChartGlobalizationSettings.GetChartTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre del Título del Gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getcharttitlename/
---
## SettableChartGlobalizationSettings.GetChartTitleName method

Obtiene el nombre del título del gráfico

```csharp
public override string GetChartTitleName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetChartTitleNameDemo
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

                // Establezca un nombre de título de gráfico personalizado
                settings.SetChartTitleName("Custom Chart Title");

                // Obtenga el nombre del título del gráfico usando GetChartTitleName
                string chartTitleName = settings.GetChartTitleName();

                // Mostrar el resultado
                Console.WriteLine("Chart Title Name: " + chartTitleName);

                // Guarda el libro de trabajo
                workbook.Save("GetChartTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetChartTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


