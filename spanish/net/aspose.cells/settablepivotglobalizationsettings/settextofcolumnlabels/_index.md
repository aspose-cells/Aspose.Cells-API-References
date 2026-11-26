---
title: "SettablePivotGlobalizationSettings.SetTextOfColumnLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto de la etiqueta Column Labels en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.SetTextOfColumnLabels method

Obtiene el texto de la etiqueta "Column Labels" en la tabla dinámica.

```csharp
public void SetTextOfColumnLabels(string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| texto | String | El texto de las etiquetas de columna |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfColumnLabelsWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo (solo para contexto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // Crear una instancia de SettablePivotGlobalizationSettings
                SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

                // Establecer texto personalizado para la etiqueta "Column Labels"
                string customColumnLabel = "My Column Headers";
                settings.SetTextOfColumnLabels(customColumnLabel);

                // Recuperar el texto actual para verificar el cambio
                string currentLabel = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Column Labels text is now: \"{currentLabel}\"");

                // Guardar el libro de trabajo (no se requiere tabla dinámica para esta demostración)
                workbook.Save("SetTextOfColumnLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


