---
title: "SettableChartGlobalizationSettings.SetOtherName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el nombre de otras etiquetas para el Gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setothername/
---
## SettableChartGlobalizationSettings.SetOtherName method

Establece el nombre de las etiquetas "Other" para el gráfico

```csharp
public void SetOtherName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetOtherNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos mínimos para contexto
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(150);

            try
            {
                // Crea una instancia de SettableChartGlobalizationSettings
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establecer un nombre personalizado para la etiqueta "Other"
                settings.SetOtherName("Miscellaneous Items");

                // Verifique la configuración obteniendo el valor
                string otherName = settings.GetOtherName();
                Console.WriteLine("Other Name set to: " + otherName);

                // Guarda el libro de trabajo
                workbook.Save("SetOtherNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOtherName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


