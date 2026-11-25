---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo locale di Anni"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

Ottiene il testo locale di "Years".

```csharp
public virtual string GetTextOfYears()
```

### Esempi

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
            // Crea impostazioni di globalizzazione personalizzate
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // Dimostra il metodo GetTextOfYears
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // Restituisce testo personalizzato per l'etichetta "Years"
            return "Custom Years Label";
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


