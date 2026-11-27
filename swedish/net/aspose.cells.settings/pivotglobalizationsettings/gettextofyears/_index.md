---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotGlobalizationSettings-metoden. Hämtar den lokala texten för år"
type: docs
url: /sv/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

Hämtar den lokala texten för "Years".

```csharp
public virtual string GetTextOfYears()
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfYearsDemo
    {
        public static void Run()
        {
            // Skapa anpassade globaliseringsinställningar
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demonstrera metoden GetTextOfYears
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // Returnera anpassad text för etiketten "Years"
            return "Custom Years Label";
        }
    }
}
```

### Se även

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


