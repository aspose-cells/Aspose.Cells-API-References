---
title: "SettableGlobalizationSettings.SetStandardFunctionName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings‑metoden. Ställer in den lokalanpassade funktionsnamnet enligt det givna standardfunktionsnamnet"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/setstandardfunctionname/
---
## SettableGlobalizationSettings.SetStandardFunctionName method

Ställer in det lokalberoende funktionsnamnet enligt det givna standardfunktionsnamnet.

```csharp
public void SetStandardFunctionName(string localName, string standardName, bool bidirectional)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| localName | String | Lokalberoende funktionsnamn |
| standardName | String | Standard (en-US‑locale) funktionsnamn. |
| bidirectional | Boolean | Om standardfunktionsnamnet ska mappas till lokalt funktionsnamn automatiskt. Om sant kommer standardnamnet att mappas till lokalt namn automatiskt så att användaren inte behöver anropa [`SetLocalFunctionName`](../setlocalfunctionname/) igen för samma standard‑ och lokala namnpar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodSetStandardFunctionNameWithStringStringBooleanDemo
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
                // Anropa SetStandardFunctionName för att mappa ett lokalt funktionsnamn till standardnamn
                settings.SetStandardFunctionName("LOCAL_SUM", "SUM", true);

                // Applicera inställningarna på arbetsboken
                workbook.Settings.GlobalizationSettings = settings;

                // Skapa en formel med det lokala funktionsnamnet
                worksheet.Cells["A1"].Formula = "=LOCAL_SUM(B1:B3)";
                worksheet.Cells["B1"].Value = 10;
                worksheet.Cells["B2"].Value = 20;
                worksheet.Cells["B3"].Value = 30;

                // Beräkna formeln
                workbook.CalculateFormula();

                Console.WriteLine("Formula with local function name 'LOCAL_SUM' calculated successfully.");
                Console.WriteLine($"Result: {worksheet.Cells["A1"].Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetStandardFunctionName method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("SetStandardFunctionNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


