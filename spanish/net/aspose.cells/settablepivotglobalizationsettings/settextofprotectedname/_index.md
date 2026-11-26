---
title: "SettablePivotGlobalizationSettings.SetTextOfProtectedName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Establece el texto para un nombre protegido específico"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/settextofprotectedname/
---
## SettablePivotGlobalizationSettings.SetTextOfProtectedName method

Establece el texto para un nombre protegido específico.

```csharp
public void SetTextOfProtectedName(string protectedName, string text)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectedName | String | El nombre protegido en la PivotTable. |
| texto | String | Los nombres protegidos locales de la PivotTable. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfProtectedNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de muestra para el contexto
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Crear una instancia de SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Establecer texto personalizado para un nombre protegido
                settings.SetTextOfProtectedName("Sum", "Custom Sum Label");

                // Verificar el cambio obteniendo el texto actual
                string currentText = settings.GetTextOfProtectedName("Sum");
                Console.WriteLine($"Text for protected name 'Sum': {currentText}");

                // Guarda el libro de trabajo para demostrar una ejecución exitosa
                workbook.Save("SetTextOfProtectedNameDemo.xlsx");
                Console.WriteLine("SetTextOfProtectedName method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


