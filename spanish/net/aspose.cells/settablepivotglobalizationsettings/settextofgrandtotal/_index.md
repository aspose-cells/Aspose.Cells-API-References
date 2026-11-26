---
title: "SettablePivotGlobalizationSettings.SetTextOfGrandTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta Grand Total en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofgrandtotal/
---
## SettablePivotGlobalizationSettings.SetTextOfGrandTotal method

Establece el texto de la etiqueta "Grand Total" en la tabla dinámica.

```csharp
public void SetTextOfGrandTotal(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfGrandTotalWithStringDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo (solo contexto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // Instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Establece un texto personalizado para la etiqueta "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Recupera el texto actualizado de la etiqueta para verificar el cambio
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Guarda el libro de trabajo solo para demostrar que el código se ejecuta sin errores
                workbook.Save("SetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


