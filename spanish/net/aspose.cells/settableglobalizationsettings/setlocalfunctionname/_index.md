---
title: "SettableGlobalizationSettings.SetLocalFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de función dependiente de la configuración regional que corresponde al nombre de función estándar dado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setlocalfunctionname/
---
## SettableGlobalizationSettings.SetLocalFunctionName method

Establece el nombre de función dependiente de la configuración regional correspondiente al nombre de función estándar dado.

```csharp
public void SetLocalFunctionName(string standardName, string localName, bool bidirectional)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | String | Nombre de función estándar (configuración regional en-US). |
| localName | String | Nombre de función dependiente de la configuración regional |
| bidirectional | Boolean | Indica si mapear el nombre de función local al nombre de función estándar automáticamente. Si es verdadero, el nombre local se mapeará al nombre estándar automáticamente, de modo que el usuario no necesite llamar a [`SetStandardFunctionName`](../setstandardfunctionname/) nuevamente para el mismo par de nombres estándar y local. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear configuraciones de globalización
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Llamar a SetLocalFunctionName para mapear el nombre de función estándar al nombre local
                settings.SetLocalFunctionName("SUM", "SOMMA", true); // Italian localization for SUM function
                settings.SetLocalFunctionName("AVERAGE", "MEDIA", true); // Italian localization for AVERAGE function

                // Aplicar la configuración al workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Crear fórmulas usando tanto nombres estándar como localizados
                worksheet.Cells["A1"].Formula = "=SUM(B1:B5)";
                worksheet.Cells["A2"].Formula = "=SOMMA(B1:B5)";
                worksheet.Cells["A3"].Formula = "=AVERAGE(B1:B5)";
                worksheet.Cells["A4"].Formula = "=MEDIA(B1:B5)";

                // Calcular fórmulas
                workbook.CalculateFormula();

                Console.WriteLine("SetLocalFunctionName executed successfully with parameters (String, String, Boolean)");
                Console.WriteLine("Standard and localized function names work equivalently in formulas.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalFunctionName method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodSetLocalFunctionNameWithStringStringBooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


