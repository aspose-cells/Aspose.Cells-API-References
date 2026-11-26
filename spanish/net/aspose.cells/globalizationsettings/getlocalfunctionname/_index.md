---
title: "GlobalizationSettings.GetLocalFunctionName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el nombre de función dependiente de la configuración regional según el nombre de función estándar proporcionado"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getlocalfunctionname/
---
## GlobalizationSettings.GetLocalFunctionName method

Obtiene el nombre de la función dependiente de la configuración regional según el nombre estándar de la función proporcionado.

```csharp
public virtual string GetLocalFunctionName(string standardName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| standardName | String | Nombre de función estándar (configuración regional en-US). |

### Valor de retorno

Nombre de función dependiente de la configuración regional. La configuración regional fue especificada por el Workbook para el cual se utiliza esta configuración.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetLocalFunctionNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            // Agregar datos de ejemplo
            worksheet.Cells["B1"].PutValue(5);
            worksheet.Cells["B2"].PutValue(15);

            // Crear fórmula con nombre de función localizado
            Cell cell = worksheet.Cells["B3"];
            cell.Formula = "=LOCALSUM(B1:B2)";

            try
            {
                workbook.CalculateFormula();
                Console.WriteLine($"Calculation result using localized function: {cell.DoubleValue}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("GlobalizationSettingsFunctionDemo.xlsx");
        }

        private class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetLocalFunctionName(string standardName)
            {
                if (standardName == "SUM")
                {
                    return "LOCALSUM";
                }
                return base.GetLocalFunctionName(standardName);
            }
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


