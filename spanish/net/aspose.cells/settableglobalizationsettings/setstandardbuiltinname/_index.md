---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Establece el nombre de función dependiente de la configuración regional según el nombre de función estándar dado.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | String | Nombre de función dependiente de la configuración regional |
| standardName | String | Nombre de función estándar (configuración regional en-US). |
| bidirectional | Boolean | Si se debe mapear el texto del nombre estándar al texto del nombre local automáticamente. Si es verdadero, el texto del nombre estándar se mapeará al texto del nombre local automáticamente, de modo que el usuario no necesite llamar a [`SetLocalBuiltInName`](../setlocalbuiltinname/) nuevamente para el mismo par de nombres estándar y local. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer la configuración de globalización para el libro de trabajo
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llame a SetStandardBuiltInName para mapear un nombre local a un nombre estándar incorporado
                // Parámetros: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Demuestre el efecto usando el nombre local en una fórmula
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Calcule la fórmula para mostrar que funciona con el nombre local
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


