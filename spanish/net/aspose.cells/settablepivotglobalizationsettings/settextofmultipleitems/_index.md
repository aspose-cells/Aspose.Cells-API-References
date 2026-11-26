---
title: "SettablePivotGlobalizationSettings.SetTextOfMultipleItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto de la etiqueta Multiple Items en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofmultipleitems/
---
## SettablePivotGlobalizationSettings.SetTextOfMultipleItems method

Establece el texto de la etiqueta "(Multiple Items)" en la tabla dinámica.

```csharp
public void SetTextOfMultipleItems(string text)
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

    public class SettablePivotGlobalizationSettingsMethodSetTextOfMultipleItemsWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos de ejemplo (opcional, solo para contexto)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Establece texto personalizado para la etiqueta "(Multiple Items)" en una tabla dinámica
                settings.SetTextOfMultipleItems("(Multiple Items Edited)");

                // Recupera y muestra el texto actualizado
                string currentText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Current text of '(Multiple Items)' label: {currentText}");

                // (Opcional) Guarda el libro de trabajo – no se requiere tabla dinámica para esta demostración
                workbook.Save("SetTextOfMultipleItemsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


