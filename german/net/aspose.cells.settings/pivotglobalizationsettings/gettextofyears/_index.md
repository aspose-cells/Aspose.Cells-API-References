---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den lokalen Text für Jahre zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

Ruft den lokalen Text von "Years" ab.

```csharp
public virtual string GetTextOfYears()
```

### Beispiele

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
            // Erstelle benutzerdefinierte Globalisierungseinstellungen
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Demonstriere die Methode GetTextOfYears
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // Gibt benutzerdefinierten Text für das Label "Years" zurück
            return "Custom Years Label";
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


