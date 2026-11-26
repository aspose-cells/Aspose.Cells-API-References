---
title: "SettablePivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettablePivotGlobalizationSettings. Obtiene el texto para el nombre protegido especificado"
type: docs
url: /es/net/aspose.cells/settablepivotglobalizationsettings/gettextofprotectedname/
---
## SettablePivotGlobalizationSettings.GetTextOfProtectedName method

Obtiene el texto para el nombre protegido especificado.

```csharp
public override string GetTextOfProtectedName(string protectedName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| protectedName | String | El nombre protegido en la PivotTable. |

### Valor de retorno

Los nombres protegidos locales de la PivotTable.

### Observaciones

En Ms Excel, algunos nombres no pueden usarse como nombre de PivotFields en la PivotTable. Son diferentes según la región; el usuario puede especificarlos explícitamente de acuerdo con la región utilizada.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfProtectedNameDemo
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
                // Establecer un texto personalizado para un nombre protegido
                settings.SetTextOfProtectedName("Sum", "Total Sum");

                // Obtener el texto del nombre protegido
                string protectedNameText = settings.GetTextOfProtectedName("Sum");

                Console.WriteLine($"Text for protected name 'Sum': {protectedNameText}");

                // Guarda el libro de trabajo
                workbook.Save("GetTextOfProtectedNameDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


