---
title: "SettableGlobalizationSettings.SetStandardBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metoden. Ställer in den lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setstandardbuiltinname/
---
## SettableGlobalizationSettings.SetStandardBuiltInName method

Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet.

```csharp
public void SetStandardBuiltInName(string localName, string standardName, bool bidirectional)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | String | Lokalberoende funktionsnamn |
| standardName | String | Standard (en-US‑locale) funktionsnamn. |
| bidirectional | Boolean | Om standardnamntexten ska mappas till lokal namntext automatiskt. Om sant kommer standardnamntexten att mappas till lokal namntext automatiskt så att användaren inte behöver anropa [`SetLocalBuiltInName`](../setlocalbuiltinname/) igen för samma standard‑ och lokala namnpar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardBuiltInNameWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa anpassade globaliseringsinställningar
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // Ställ in globaliseringsinställningarna för arbetsboken
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // Anropa SetStandardBuiltInName för att mappa ett lokalt namn till ett standardinbyggt namn
                // Parametrar: localName, standardName, bidirectional
                settings.SetStandardBuiltInName("MyLocalName", "SUM", true);
                
                Console.WriteLine("SetStandardBuiltInName executed successfully with parameters (\"MyLocalName\", \"SUM\", true)");
                
                // Demonstrera effekten genom att använda det lokala namnet i en formel
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=MyLocalName(A1:A2)";
                
                // Beräkna formeln för att visa att den fungerar med det lokala namnet
                workbook.CalculateFormula();
                Console.WriteLine("Result of formula with local name: " + worksheet.Cells["A3"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardBuiltInName method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SetStandardBuiltInNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


