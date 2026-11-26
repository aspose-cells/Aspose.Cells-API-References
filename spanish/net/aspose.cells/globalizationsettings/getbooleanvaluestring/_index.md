---
title: "GlobalizationSettings.GetBooleanValueString"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GlobalizationSettings. Obtiene el valor de cadena de visualización para el valor booleano de las celdas"
type: docs
url: /es/net/aspose.cells/globalizationsettings/getbooleanvaluestring/
---
## GlobalizationSettings.GetBooleanValueString method

Obtiene la cadena de visualización del valor booleano de la celda

```csharp
public virtual string GetBooleanValueString(bool bv)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| bv | Booleano | valor booleano |

### Valor de retorno

Por defecto devuelve "TRUE" para el valor verdadero y "FALSE" para el valor falso.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetBooleanValueStringWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo con configuraciones de globalización personalizadas
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomBooleanGlobalizationSettings();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demostrar GetBooleanValueString con ambos valores booleanos
                var globalizationSettings = workbook.Settings.GlobalizationSettings;
                string trueResult = globalizationSettings.GetBooleanValueString(true);
                string falseResult = globalizationSettings.GetBooleanValueString(false);

                Console.WriteLine($"GetBooleanValueString(true) returns: {trueResult}");
                Console.WriteLine($"GetBooleanValueString(false) returns: {falseResult}");

                // Aplicar valores booleanos a las celdas para mostrar el efecto en la hoja de cálculo
                worksheet.Cells["A1"].PutValue(true);
                worksheet.Cells["A2"].PutValue(false);

                workbook.Save("GlobalizationBooleanDemo.xlsx");
                Console.WriteLine("Workbook saved with custom boolean representations.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetBooleanValueString: {ex.Message}");
            }
        }
    }

    // Configuraciones de globalización personalizadas que sobrescriben la representación de cadena booleana
    public class CustomBooleanGlobalizationSettings : GlobalizationSettings
    {
        public override string GetBooleanValueString(bool bv)
        {
            return bv ? "Enabled" : "Disabled";
        }
    }
}
```

### Ver también

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


