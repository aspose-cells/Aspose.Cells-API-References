---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo PivotGlobalizationSettings. Restituisce il testo locale di Minuti"
type: docs
url: /it/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

Ottiene il testo locale di "Minutes".

```csharp
public virtual string GetTextOfMinutes()
```

### Esempi

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
            // Crea un'istanza di PivotGlobalizationSettings
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // Dimostra il metodo GetTextOfMinutes
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Dimostrazione aggiuntiva dei metodi temporali correlati per contesto
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Vedi anche

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


