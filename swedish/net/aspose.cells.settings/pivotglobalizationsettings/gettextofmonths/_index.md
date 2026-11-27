---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings‑metod. Hämtar den lokala texten för Months"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Hämtar den lokala texten för "Months".

```csharp
public virtual string GetTextOfMonths()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfMonthsDemo
    {
        public static void Run()
        {
            // Skapa anpassade globaliseringsinställningar
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demonstrera GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // Returnera anpassad lokaliserad text för "Months"
            return "Custom Months Label";
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


