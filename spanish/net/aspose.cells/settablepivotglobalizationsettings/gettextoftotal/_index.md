---
title: "SettablePivotGlobalizationSettings.GetTextOfTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto de la etiqueta Total en la PivotTable. Necesita sobrescribir este método cuando la PivotTable contiene dos o más PivotFields en el área de datos"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextoftotal/
---
## SettablePivotGlobalizationSettings.GetTextOfTotal method

Obtiene el texto de la etiqueta "Total" en la tabla dinámica. Necesita sobrescribir este método cuando la tabla dinámica contiene dos o más PivotFields en el área de datos.

```csharp
public override string GetTextOfTotal()
```

### Valor de retorno

El texto de la etiqueta "Total"

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfTotalDemo
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
                // Establecer texto personalizado para la etiqueta "Total"
                settings.SetTextOfTotal("Custom Total");

                // Obtener el texto de la etiqueta "Total"
                string totalText = settings.GetTextOfTotal();

                Console.WriteLine($"Text of Total: {totalText}");

                // Guarda el libro de trabajo
                workbook.Save("GetTextOfTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfTotal: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


