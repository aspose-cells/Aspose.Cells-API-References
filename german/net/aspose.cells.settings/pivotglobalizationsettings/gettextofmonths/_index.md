---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings Methode. Gibt den lokalen Text der Monate zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Ruft den lokalen Text von "Months" ab.

```csharp
public virtual string GetTextOfMonths()
```

### Beispiele

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
            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demonstriere GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // Gib benutzerdefinierten lokalisierten Text für "Months" zurück
            return "Custom Months Label";
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


