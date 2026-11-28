---
title: "PivotGlobalizationSettings.GetTextOfMonths"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Ayların yerel metnini alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofmonths/
---
## PivotGlobalizationSettings.GetTextOfMonths method

"Months" ifadesinin yerel metnini alır.

```csharp
public virtual string GetTextOfMonths()
```

### Örnekler

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
            // Özel küreselleşme ayarları oluşturun
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // GetTextOfMonths yöntemini göster
            Console.WriteLine("Custom Months Text: " + customSettings.GetTextOfMonths());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfMonths()
        {
            // "Months" için özel yerelleştirilmiş metni döndür
            return "Custom Months Label";
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


