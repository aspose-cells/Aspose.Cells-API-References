---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Restituisce il testo locale di Mesi"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

Ottiene il testo locale di "Months".

```csharp
public virtual string GetTextOfMonths()
```

### Esempi

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
            // Crea impostazioni di globalizzazione personalizzate
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Dimostra GetTextOfMonths
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // Restituisce testo localizzato personalizzato per "Mesi"
            return "Custom Months Label";
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


