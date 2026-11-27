---
title: "PivotGlobalizationSettings.GetTextOf4Quaters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metod. Hämtar den lokala texten för 4 Quarters"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextof4quaters/
---
## PivotGlobalizationSettings.GetTextOf4Quaters method

Hämtar den lokala texten för 4 kvartal.

```csharp
[Obsolete("Use PivotGlobalizationSettings.GetTextOf4Quarters() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string[] GetTextOf4Quaters()
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället PivotGlobalizationSettings.GetTextOf4Quarters()‑metoden. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Settings;
    using System;

    public class PivotGlobalizationSettingsMethodGetTextOf4QuatersDemo
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
                // Anropa GetTextOf4Quaters-metoden
                string[] quarterNames = customGlobalizationSettings.GetTextOf4Quaters();

                // Skriv ut kvartalsnamnen till konsolen
                Console.WriteLine("Names of 4 quarters:");
                foreach (string quarterName in quarterNames)
                {
                    Console.WriteLine(quarterName);
                }

                // Lägg till kvartalsnamnen i kalkylbladet
                for (int i = 0; i < quarterNames.Length; i++)
                {
                    worksheet.Cells[i, 0].PutValue(quarterNames[i]);
                }

                Console.WriteLine("Method executed successfully. Quarter names added to worksheet.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTextOf4Quaters method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetTextOf4QuatersDemo.xlsx");
        }
    }

    // Anpassad implementation av PivotGlobalizationSettings för att åsidosätta GetTextOf4Quaters
    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string[] GetTextOf4Quaters()
        {
            // Returnera anpassade kvartalsnamn
            return new string[] { "First Quarter", "Second Quarter", 
                               "Third Quarter", "Fourth Quarter" };
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


