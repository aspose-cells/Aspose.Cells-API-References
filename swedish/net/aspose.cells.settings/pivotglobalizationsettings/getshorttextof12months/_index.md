---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar alla kortformaterade strängar för 12 månader"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

Hämtar alla kortformaterade strängar för 12 månader.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en anpassad globaliseringsinställningsklass som ärver från PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Anropa metoden GetShortTextOf12Months
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Skriv ut månadsnamnen till konsolen
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Lägg till månadsnamnen i kalkylbladet
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

            // Spara resultatet
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // Anpassad implementation av PivotGlobalizationSettings för att åsidosätta GetShortTextOf12Months
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Returnera anpassade korta månadsnamn
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


