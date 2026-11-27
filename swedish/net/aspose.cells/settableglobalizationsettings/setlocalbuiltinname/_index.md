---
title: "SettableGlobalizationSettings.SetLocalBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metod. Anger den lokalberoende texten för det inbyggda namnet med given standardnamnstext"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setlocalbuiltinname/
---
## SettableGlobalizationSettings.SetLocalBuiltInName method

Ställer in den lokalberoende texten för det inbyggda namnet med given standard name text.

```csharp
public void SetLocalBuiltInName(string standardName, string localName, bool bidirectional)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | String | Standard (en-US‑lokal) namntext för det inbyggda namnet. |
| localName | String | Lokalberoende namntext |
| bidirectional | Boolean | Om den lokala namntexten ska mappas till standardnamntext automatiskt. Om sant kommer den lokala namntexten att mappas till standardnamntext automatiskt så att användaren inte behöver anropa [`SetStandardBuiltInName`](../setstandardbuiltinname/) igen för samma standard‑ och lokala namnpar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetLocalBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Anropa SetLocalBuiltInName för att mappa ett standardinbyggt namn till ett lokalt namn
                settings.SetLocalBuiltInName("SUM", "LOCAL_SUM", true);

                // Applicera inställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Skapa en formel med det standardinbyggda namnet
                worksheet.Cells["A1"].Formula = "=SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 5;
                worksheet.Cells["B2"].Value = 10;
                worksheet.Cells["B3"].Value = 15;

                // Beräkna formeln
                workbook.CalculateFormula();

                Console.WriteLine("Formula with standard built-in name 'SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");

                // Verifiera den lokala namn-mappningen
                string localName = settings.GetLocalBuiltInName("SUM");
                Console.WriteLine($"Local name for 'SUM': {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetLocalBuiltInName method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


