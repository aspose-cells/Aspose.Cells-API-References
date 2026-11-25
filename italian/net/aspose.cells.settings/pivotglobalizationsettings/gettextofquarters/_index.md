---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Ottiene il testo locale dei trimestri"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

Ottieni il testo locale di "Quarters".

```csharp
public virtual string GetTextOfQuarters()
```

### Esempi

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
            // Crea un'istanza delle impostazioni di globalizzazione
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // Dimostra il metodo GetTextOfQuarters
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Mostra altre etichette di periodi di tempo correlati per il contesto
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


