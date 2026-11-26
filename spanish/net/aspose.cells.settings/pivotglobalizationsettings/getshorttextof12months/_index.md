---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotGlobalizationSettings. Obtiene todas las cadenas cortas formateadas de los 12 meses"
type: docs
url: /es/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

Obtiene todas las cadenas de formato corto de los 12 meses.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetShortTextOf12MonthsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cree una clase de configuración de globalización personalizada que herede de PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Llame al método GetShortTextOf12Months
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Muestre los nombres de los meses en la consola
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Agregue los nombres de los meses a la hoja de cálculo
                for (int i = 0; i < monthShortNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(monthShortNames[i]);
                }

                Console.WriteLine("Method executed successfully. Month names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetShortTextOf12Months method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // Implementación personalizada de PivotGlobalizationSettings para sobrescribir GetShortTextOf12Months
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Devuelva nombres de meses cortos personalizados
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### Ver también

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


