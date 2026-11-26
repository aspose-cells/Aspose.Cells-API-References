---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | String | Nombre de función dependiente de la configuración regional |
| standardName | String | Nombre de función estándar (configuración regional en-US). |
| bidirectional | Boolean | Indica si se debe mapear el nombre de función estándar al nombre de función local automáticamente. Si es verdadero, el nombre estándar se mapeará al nombre local automáticamente, de modo que el usuario no necesite llamar a [`SetLocalFunctionName`](../setlocalfunctionname/) nuevamente para el mismo par de nombres estándar y local. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Llamar a SetStandardFunctionName para mapear un nombre de función local al nombre estándar
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Aplicar la configuración al libro de trabajo
                workbook.Settings.GlobalizationSettings = settings;

                // Crear una fórmula usando el nombre de función local
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Calcular la fórmula
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


