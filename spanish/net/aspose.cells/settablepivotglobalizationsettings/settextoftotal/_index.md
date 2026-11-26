---
title: "SettablePivotGlobalizationSettings.SetTextOfTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta Total en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextoftotal/
---
## SettablePivotGlobalizationSettings.SetTextOfTotal method

Establece el texto de la etiqueta "Total" en la tabla dinámica.

```csharp
public void SetTextOfTotal(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | texto personalizado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfTotalWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de muestra para el contexto
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B3"].Value = 200;

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Obtén el texto predeterminado "Total"
                string defaultTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Default Total text: {defaultTotalText}");

                // Establece un texto personalizado para "Total"
                settings.SetTextOfTotal("Custom Total Label");

                // Verificar el cambio
                string updatedTotalText = settings.GetTextOfTotal();
                Console.WriteLine($"Updated Total text: {updatedTotalText}");

                // Guarda el libro de trabajo
                workbook.Save("SetTextOfTotalDemo.xlsx");
                Console.WriteLine("SetTextOfTotal method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


