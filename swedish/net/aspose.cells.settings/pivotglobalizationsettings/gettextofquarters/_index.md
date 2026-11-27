---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metod. Hämta den lokala texten för Quarters"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Hämta den lokala texten för "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfQuartersDemo
    {
        public static void Run()
        {
            // Skapa en instans av globaliseringsinställningar
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstrera GetTextOfQuarters‑metoden
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Visa andra relaterade tidsperiodetiketter för kontext
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


