---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotGlobalizationSettings Methode. Gibt den lokalen Text der Quartale zurück"
type: docs
url: /de/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Rufe den lokalen Text von "Quarters" ab.

```csharp
public virtual string GetTextOfQuarters()
```

### Beispiele

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
            // Erstellen Sie eine Globalisierungs‑Einstellungsinstanz
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Demonstriere die GetTextOfQuarters-Methode
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Weitere verwandte Zeitperiodenbeschriftungen für den Kontext anzeigen
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Siehe auch

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


