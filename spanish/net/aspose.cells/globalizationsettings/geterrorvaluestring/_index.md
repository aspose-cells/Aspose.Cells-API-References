---
title: "GlobalizationSettings.GetErrorValueString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene la cadena de visualización para el valor de error de la celda"
type: docs
url: /es/net/aspose.cells/globalizationsettings/geterrorvaluestring/
---
## GlobalizationSettings.GetErrorValueString method

Obtiene la cadena de visualización del valor de error de la celda

```csharp
public virtual string GetErrorValueString(string err)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| err | String | valores de error como #VALUE!,#NAME? |

### Valor de retorno

Por defecto devuelve el propio valor de error

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetErrorValueStringWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer configuraciones de globalización personalizadas
            workbook.Settings.GlobalizationSettings = new CustomErrorGlobalizationSettings();

            // Crear escenario de error: división por cero
            Cell cell = worksheet.Cells["A1"];
            cell.Formula = "=1/0";  // This will generate #DIV/0! error

            try
            {
                workbook.CalculateFormula();
                string errorValue = cell.DisplayStringValue;
                
                Console.WriteLine($"Error display value: {errorValue}");
                Console.WriteLine("Method executed successfully - see custom error mapping");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetErrorValueString method: {ex.Message}");
            }

            workbook.Save("MethodGetErrorValueStringDemo.xlsx");
        }
    }

    public class CustomErrorGlobalizationSettings : GlobalizationSettings
    {
        public override string GetErrorValueString(string err)
        {
            // Mapeos personalizados de valores de error
            return err switch
            {
                "#DIV/0!" => "Custom Division Error",
                "#VALUE!" => "Custom Type Mismatch",
                "#NAME?" => "Custom Identifier Error",
                _ => base.GetErrorValueString(err)
            };
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


