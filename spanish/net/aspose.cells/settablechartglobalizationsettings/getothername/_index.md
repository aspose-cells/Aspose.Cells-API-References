---
title: "SettableChartGlobalizationSettings.GetOtherName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableChartGlobalizationSettings. Obtiene el nombre de las etiquetas Other para el gráfico"
type: docs
url: /es/net/aspose.cells/settablechartglobalizationsettings/getothername/
---
## SettableChartGlobalizationSettings.GetOtherName method

Obtiene el nombre de las etiquetas "Other" para el gráfico

```csharp
public override string GetOtherName()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableChartGlobalizationSettingsMethodGetOtherNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos mínimos (opcional, solo para un libro de trabajo completo)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(250);

            try
            {
                // Instanciar el objeto de configuración de globalización
                SettableChartGlobalizationSettings settings = new SettableChartGlobalizationSettings();

                // Establecer un nombre personalizado para la etiqueta "Other"
                settings.SetOtherName("Custom Other Label");

                // Recuperar el nombre usando GetOtherName
                string otherName = settings.GetOtherName();

                Console.WriteLine("Other Name retrieved: " + otherName);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetOtherName: {ex.Message}");
            }

            // Guardar el libro de trabajo (la configuración no está directamente adjunta al gráfico en esta demostración)
            workbook.Save("GetOtherNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableChartGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


