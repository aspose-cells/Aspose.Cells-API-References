---
title: "SettableChartGlobalizationSettings.GetLegendTotalName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre del Total para la Leyenda"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getlegendtotalname/
---
## SettableChartGlobalizationSettings.GetLegendTotalName method

Obtiene el nombre de total para la leyenda

```csharp
public override string GetLegendTotalName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetLegendTotalNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Primero establezca un nombre de total de leyenda personalizado
                settings.SetLegendTotalName("Custom Total Label");

                // Llame al método GetLegendTotalName para recuperar el valor
                string legendTotalName = settings.GetLegendTotalName();

                // Mostrar el resultado
                Console.WriteLine("Legend Total Name: " + legendTotalName);

                // Guarda el libro de trabajo
                workbook.Save("GetLegendTotalNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLegendTotalName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


