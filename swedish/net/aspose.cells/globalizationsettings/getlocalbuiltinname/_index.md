---
title: "GlobalizationSettings.GetLocalBuiltInName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GlobalizationSettings-metoden. Hämtar den lokalanpassade texten för builtin Name enligt given standardtext"
type: docs
url: /sv/net/aspose.cells/globalizationsettings/getlocalbuiltinname/
---
## GlobalizationSettings.GetLocalBuiltInName method

Hämtar den lokalanpassade texten för inbyggt namn enligt given standardtext.

```csharp
public virtual string GetLocalBuiltInName(string standardName)
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

    public class GlobalizationSettingsMethodGetLocalBuiltInNameWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                string standardName = "Total";
                string localizedName = ((CustomGlobalizationSettings)workbook.Settings.GlobalizationSettings).GetLocalBuiltInName(standardName);

                Console.WriteLine($"Standard Name: {standardName}");
                Console.WriteLine($"Localized Name: {localizedName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetLocalBuiltInName method: {ex.Message}");
            }

            workbook.Save("LocalizedBuiltInNameDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetLocalBuiltInName(string standardName)
        {
            switch (standardName)
            {
                case "Total":
                    return "LocalizedTotal";
                case "Average":
                    return "LocalizedAverage";
                default:
                    return base.GetLocalBuiltInName(standardName);
            }
        }
    }
}
```

### Se även

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


