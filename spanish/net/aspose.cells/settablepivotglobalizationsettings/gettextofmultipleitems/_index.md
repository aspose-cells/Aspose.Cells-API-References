---
title: "SettablePivotGlobalizationSettings.GetTextOfMultipleItems"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto de la etiqueta Multiple Items en la PivotTable"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofmultipleitems/
---
## SettablePivotGlobalizationSettings.GetTextOfMultipleItems method

Obtiene el texto de la etiqueta "(Multiple Items)" en la tabla dinámica.

```csharp
public override string GetTextOfMultipleItems()
```

### Valor de retorno

El texto de la etiqueta "(Multiple Items)"

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfMultipleItemsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de muestra para el contexto
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
                // Obtener el texto predeterminado para múltiples elementos
                string multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Default text for multiple items: {multipleItemsText}");

                // Establecer un texto personalizado para múltiples elementos
                settings.SetTextOfMultipleItems("(Multiple Items Custom)");
                multipleItemsText = settings.GetTextOfMultipleItems();
                Console.WriteLine($"Updated text for multiple items: {multipleItemsText}");

                // Guarda el libro de trabajo
                workbook.Save("GetTextOfMultipleItemsDemo.xlsx");
                Console.WriteLine("GetTextOfMultipleItems method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfMultipleItems: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


