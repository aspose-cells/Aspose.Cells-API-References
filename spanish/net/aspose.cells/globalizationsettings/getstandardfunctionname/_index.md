---
title: "GlobalizationSettings.GetStandardFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de función estándar según el nombre de función dependiente de la configuración regional proporcionado"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getstandardfunctionname/
---
## GlobalizationSettings.GetStandardFunctionName method

Obtiene el nombre estándar de la función según el nombre de función dependiente de la configuración regional proporcionado.

```csharp
public virtual string GetStandardFunctionName(string localName)
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

    public class GlobalizationSettingsMethodGetStandardFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Preparar datos de ejemplo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(15);
            
            // Crear configuraciones de globalización personalizadas y asignarlas al libro de trabajo
            var customSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = customSettings;

            try
            {
                // Demostrar GetStandardFunctionName con el nombre de función SUM en alemán
                string localName = "SUMME";
                string standardName = customSettings.GetStandardFunctionName(localName);
                
                Console.WriteLine($"Local function name: {localName}");
                Console.WriteLine($"Standard function name: {standardName}");

                // Aplicar el nombre de función localizado en la fórmula
                worksheet.Cells["A3"].Formula = "=SUMME(A1:A2)";
                workbook.CalculateFormula();
                
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardFunctionName method: {ex.Message}");
            }

            workbook.Save("MethodGetStandardFunctionNameDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetStandardFunctionName(string localName)
            {
                // Convertir el nombre de función en alemán al inglés estándar
                if (localName.Equals("SUMME", StringComparison.OrdinalIgnoreCase))
                {
                    return "SUM";
                }
                return base.GetStandardFunctionName(localName);
            }
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


