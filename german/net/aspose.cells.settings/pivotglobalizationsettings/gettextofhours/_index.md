---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings-Methode. Gibt den lokalen Text der Stunden zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

Ruft den lokalen Text von "Hours" ab.

```csharp
public virtual string GetTextOfHours()
```

### Beispiele

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
            // Erstelle eine Instanz von PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // GetTextOfHours-Methode demonstrieren
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // Zusätzliche Demonstration von verwandten Zeitmethoden
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


