---
title: "PivotGlobalizationSettings.GetTextOfMinutes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Dakikaların yerel metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofminutes/
---
## PivotGlobalizationSettings.GetTextOfMinutes method

"Minutes" ifadesinin yerel metnini alır.

```csharp
public virtual string GetTextOfMinutes()
```

### Örnekler

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
            // PivotGlobalizationSettings örneği oluştur
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

            // GetTextOfMinutes yöntemini göster
            Console.WriteLine("Text of Minutes: " + globalizationSettings.GetTextOfMinutes());

            // Bağlam için ilgili zaman yöntemlerine ek gösterim
            Console.WriteLine("Text of Hours: " + globalizationSettings.GetTextOfHours());
            Console.WriteLine("Text of Seconds: " + globalizationSettings.GetTextOfSeconds());
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


