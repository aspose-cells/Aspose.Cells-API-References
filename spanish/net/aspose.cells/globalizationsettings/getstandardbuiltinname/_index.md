---
title: "GlobalizationSettings.GetStandardBuiltInName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el texto estándar del nombre incorporado según el texto dependiente de la configuración regional proporcionado"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getstandardbuiltinname/
---
## GlobalizationSettings.GetStandardBuiltInName method

Obtiene el texto estándar del Nombre incorporado según el texto dependiente de la configuración regional proporcionado.

```csharp
public virtual string GetStandardBuiltInName(string localName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| localName | String | Texto dependiente de la configuración regional del nombre incorporado. La configuración regional fue especificada por el Libro de trabajo para el cual se utilizan estos ajustes. |

### Valor de retorno

Texto estándar (configuración regional en-US).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetStandardBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Inicializar configuraciones de globalización personalizadas y asignarlas al libro de trabajo
            var globalizationSettings = new CustomGlobalizationSettings();
            workbook.Settings.GlobalizationSettings = globalizationSettings;

            // Parámetro de prueba para GetStandardBuiltInName
            string localFunctionName = "MyLocalSum";
            
            try
            {
                // Llamar a GetStandardBuiltInName con el nombre de función local
                string standardName = globalizationSettings.GetStandardBuiltInName(localFunctionName);
                Console.WriteLine($"Local name: '{localFunctionName}' => Standard name: '{standardName}'");

                // Demostrar el efecto usando el nombre local en una fórmula
                worksheet.Cells["A1"].Value = 5;
                worksheet.Cells["A2"].Value = 7;
                worksheet.Cells["A3"].Formula = $"{localFunctionName}(A1:A2)";

                // Calcular la fórmula para mostrar la interpretación correcta
                workbook.CalculateFormula();
                Console.WriteLine($"Formula result: {worksheet.Cells["A3"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetStandardBuiltInName: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("GlobalizationGetStandardBuiltInNameDemo.xlsx");
        }
    }

    // Configuraciones de globalización personalizadas que sobrescriben GetStandardBuiltInName
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetStandardBuiltInName(string localName)
        {
            // Mapear el nombre de función local personalizado a la SUM estándar
            if (localName.Equals("MyLocalSum", StringComparison.OrdinalIgnoreCase))
            {
                return "SUM";
            }
            return base.GetStandardBuiltInName(localName);
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


