---
title: "SettableChartGlobalizationSettings.SetAxisTitleName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Establece el nombre del Título para el Eje"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/setaxistitlename/
---
## SettableChartGlobalizationSettings.SetAxisTitleName method

Establece el nombre del título para el eje

```csharp
public void SetAxisTitleName(string name)
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

    public class SettableChartGlobalizationSettingsMethodSetAxisTitleNameDemo
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

                // Establecer un nombre de título de eje personalizado
                settings.SetAxisTitleName("Custom Axis Title");

                // Verifique la configuración obteniendo el nombre del título del eje
                string axisTitleName = settings.GetAxisTitleName();
                Console.WriteLine("Axis Title Name: " + axisTitleName);

                // Guarda el libro de trabajo
                workbook.Save("SetAxisTitleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetAxisTitleName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


