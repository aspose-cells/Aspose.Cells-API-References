---
title: "SettableGlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettableGlobalizationSettings-metoden. Hämtar den lokalanpassade texten för inbyggt Name enligt given standardtext"
type: docs
url: /sv/net/aspose.cells/settableglobalizationsettings/getlocalbuiltinname/
---
## SettableGlobalizationSettings.GetLocalBuiltInName method

Hämtar den lokalanpassade texten för inbyggt namn enligt given standardtext.

```csharp
public override string GetLocalBuiltInName(string standardName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| standardName | String | Standard (en-US-lokal) text för inbyggt Name. |

### Returvärde

Lokalanpassad text. Lokalen angavs av arbetsboken för vilken dessa inställningar används.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettableGlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SettableGlobalizationSettings
            SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

            try
            {
                // Anropa GetLocalBuiltInName‑metoden med ett standardinbyggt namn
                string standardName = "SUM";
                string localName = globalizationSettings.GetLocalBuiltInName(standardName);

                // Visa resultatet
                Console.WriteLine($"Standard name: {standardName}, Local name: {localName}");

                // Ange ett anpassat lokalt namn för det standardinbyggda namnet
                globalizationSettings.SetLocalBuiltInName(standardName, "CustomSum", true);

                // Hämta det lokala namnet igen efter att det har ställts in
                localName = globalizationSettings.GetLocalBuiltInName(standardName);
                Console.WriteLine($"After setting - Standard name: {standardName}, Local name: {localName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("MethodGetLocalBuiltInNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


