---
title: "SettablePivotGlobalizationSettings.GetTextOfGrandTotal"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto de la etiqueta Grand Total en la tabla dinámica"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofgrandtotal/
---
## SettablePivotGlobalizationSettings.GetTextOfGrandTotal method

Obtiene el texto de la etiqueta "Grand Total" en la tabla dinámica.

```csharp
public override string GetTextOfGrandTotal()
```

### Valor de retorno

El texto de la etiqueta "Grand Total"

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfGrandTotalDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo (solo para contexto)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample");

            // Instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Cambia el texto predeterminado "Grand Total"
                settings.SetTextOfGrandTotal("My Custom Grand Total");

                // Recupera el texto actual "Grand Total"
                string grandTotalText = settings.GetTextOfGrandTotal();

                Console.WriteLine($"Grand Total label text: {grandTotalText}");

                // Guarda el libro de trabajo (no se crea tabla dinámica, pero el archivo se guarda para demostrar la ejecución)
                workbook.Save("GetTextOfGrandTotalDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfGrandTotal: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


