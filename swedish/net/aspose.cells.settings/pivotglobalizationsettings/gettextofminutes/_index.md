---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metod. Hämtar den lokala texten för Minutes"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

Hämtar den lokala texten för "Minutes".

```csharp
public virtual string GetTextOfMinutes()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMinutesDemo
    {
        public static void Run()
        {
            // Skapa en instans av PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstrera GetTextOfMinutes‑metoden
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Ytterligare demonstration av relaterade tidsmetoder för kontext
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


