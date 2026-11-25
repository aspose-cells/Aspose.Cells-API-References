---
title: "PivotGlobalizationSettings.GetShortTextOf12Months"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene tutte le stringhe brevi formattate dei 12 mesi"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/getshorttextof12months/
---
## PivotGlobalizationSettings.GetShortTextOf12Months method

Ottiene tutte le stringhe brevi formattate dei 12 mesi.

```csharp
public virtual string[] GetShortTextOf12Months()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una classe di impostazioni di globalizzazione personalizzata che eredita da PivotGlobalizationSettings
            var customGlobalizationSettings = new CustomPivotGlobalizationSettings();

            try
            {
                // Chiama il metodo GetShortTextOf12Months
                string[] monthShortNames = customGlobalizationSettings.GetShortTextOf12Months();

                // Stampa i nomi dei mesi sulla console
                Console.WriteLine("Short names of 12 months:");
                foreach (string monthName in monthShortNames)
                {
                    Console.WriteLine(monthName);
                }

                // Aggiungi i nomi dei mesi al foglio di lavoro
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

            // Salva il risultato
            workbook.Save("MethodGetShortTextOf12MonthsDemo.xlsx");
        }
    }

    // Implementazione personalizzata di PivotGlobalizationSettings per sovrascrivere GetShortTextOf12Months
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetShortTextOf12Months()
        {
            // Restituisce i nomi brevi dei mesi personalizzati
            return new string[] { "Jan", "Feb", "Mar", "Apr", "May", "Jun", 
                                "Jul", "Aug", "Sep", "Oct", "Nov", "Dec" };
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


