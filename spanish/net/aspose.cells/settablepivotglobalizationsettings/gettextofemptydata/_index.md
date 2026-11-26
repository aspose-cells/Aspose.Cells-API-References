---
title: "SettablePivotGlobalizationSettings.GetTextOfEmptyData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto de la etiqueta en blanco en la PivotTable"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofemptydata/
---
## SettablePivotGlobalizationSettings.GetTextOfEmptyData method

Obtiene el texto de la etiqueta "(blank)" en la tabla dinámica.

```csharp
public override string GetTextOfEmptyData()
```

### Valor de retorno

El texto de datos vacíos

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfEmptyDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Obtener el texto predeterminado para datos vacíos
                string emptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Default text for empty data: '{emptyDataText}'");

                // Establecer un texto personalizado para datos vacíos
                settings.SetTextOfEmptyData("No Data Available");

                // Obtenga el texto actualizado para datos vacíos
                string updatedEmptyDataText = settings.GetTextOfEmptyData();
                Console.WriteLine($"Updated text for empty data: '{updatedEmptyDataText}'");

                // Aplicar configuraciones al libro de trabajo
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();
                globalizationSettings.PivotSettings = settings;
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // Guarda el libro de trabajo
                workbook.Save("GetTextOfEmptyDataDemo.xlsx");
                Console.WriteLine("GetTextOfEmptyData method demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetTextOfEmptyData: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


