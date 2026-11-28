---
title: "PivotGlobalizationSettings.GetTextOfQuarters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Çeyreklerin yerel metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofquarters/
---
## PivotGlobalizationSettings.GetTextOfQuarters method

"Quarters" ifadesinin yerel metnini al.

```csharp
public virtual string GetTextOfQuarters()
```

### Örnekler

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
            // Küreselleştirme ayarları örneği oluşturun
            PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();
            
            // GetTextOfQuarters yöntemini gösterin
            Console.WriteLine("Quarter labels: " + globalizationSettings.GetTextOfQuarters());
            
            // Bağlam için diğer ilgili zaman dilimi etiketlerini gösterin
            Console.WriteLine("Year labels: " + globalizationSettings.GetTextOfYears());
            Console.WriteLine("Month labels: " + globalizationSettings.GetTextOfMonths());
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


