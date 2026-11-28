---
title: "PivotGlobalizationSettings.GetTextOfHours"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Saatlerin yerel metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofhours/
---
## PivotGlobalizationSettings.GetTextOfHours method

"Hours" ifadesinin yerel metnini alır.

```csharp
public virtual string GetTextOfHours()
```

### Örnekler

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
            // PivotGlobalizationSettings örneği oluştur
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // GetTextOfHours yöntemini gösterin
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());

            // İlgili zaman yöntemlerinin ek gösterimi
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


