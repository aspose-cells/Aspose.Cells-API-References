---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings Methode. Gibt den lokalen Text der Minuten zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

Ruft den lokalen Text von "Minutes" ab.

```csharp
public virtual string GetTextOfMinutes()
```

### Beispiele

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
            // Erstelle eine Instanz von PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Demonstriere die GetTextOfMinutes-Methode
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Zusätzliche Demonstration verwandter Zeitmethoden für den Kontext
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


