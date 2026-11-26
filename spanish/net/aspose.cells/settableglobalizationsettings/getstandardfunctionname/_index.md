---
title: "SettableGlobalizationSettings.GetStandardFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SettableGlobalizationSettings. Obtiene el nombre de función estándar según el nombre de función dependiente de la configuración regional proporcionado"
type: docs
url: /es/net/aspose.cells/settableglobalizationsettings/getstandardfunctionname/
---
## SettableGlobalizationSettings.GetStandardFunctionName method

Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado.

```csharp
public override string GetStandardFunctionName(string localName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | String | Nombre de función dependiente de la configuración regional. La configuración regional fue especificada por el Workbook para el cual se utiliza esta configuración. |

### Valor de retorno

Nombre de función estándar (configuración regional en-US).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree configuraciones de globalización personalizadas
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Establecer un mapeo de nombre de función local
            settings.SetStandardFunctionName("LocalSum", "SUM", true);

            // Aplicar la configuración al workbook
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Llamar a GetStandardFunctionName con un nombre de función local
                string standardName = settings.GetStandardFunctionName("LocalSum");
                
                // Mostrar el resultado
                Console.WriteLine($"Standard function name for 'LocalSum' is: {standardName}");

                // Utilizar la función estándar en una fórmula de celda
                worksheet.Cells["A1"].Formula = $"={standardName}(1,2,3)";
                worksheet.Cells["A2"].Value = 1;
                worksheet.Cells["A3"].Value = 2;
                worksheet.Cells["A4"].Value = 3;

                // Calcular la fórmula
                workbook.CalculateFormula();

                // Mostrar el resultado
                Console.WriteLine($"Formula result in A1: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("SettableGlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


