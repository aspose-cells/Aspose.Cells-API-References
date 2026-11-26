---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el texto dependiente de la configuración regional para el nombre incorporado con el texto del nombre estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Establece el texto dependiente de la configuración regional para el nombre incorporado con el texto de nombre estándar proporcionado.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | String | Texto del nombre estándar (configuración regional en-US) del nombre incorporado. |
| localName | String | Texto del nombre dependiente de la configuración regional |
| bidirectional | Boolean | Indica si se debe mapear el texto del nombre local al texto del nombre estándar automáticamente. Si es verdadero, el texto del nombre local se mapeará al texto del nombre estándar automáticamente, de modo que el usuario no necesite llamar a [`SetStandardBuiltInName`](../setstandardbuiltinname/) nuevamente para el mismo par de nombres estándar y local. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
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
                // Llamar a SetLocalBuiltInName para mapear un nombre incorporado estándar a un nombre local
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Aplicar la configuración al workbook
                workbook.Settings.GlobalizationSettings = settings;

                // Crear una fórmula usando el nombre incorporado estándar
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Calcular la fórmula
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Verificar el mapeo del nombre local
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


