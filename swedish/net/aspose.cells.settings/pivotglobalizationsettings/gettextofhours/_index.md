---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar den lokala texten för Timmar"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

Hämtar den lokala texten för "Hours".

```csharp
public virtual string GetTextOfHours()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfHoursDemo
    {
        public static void Run()
        {
            // Skapa en instans av PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrera GetTextOfHours-metoden
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // Ytterligare demonstration av relaterade tidsmetoder
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


