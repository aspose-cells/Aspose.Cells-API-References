---
title: "PivotGlobalizationSettings.GetTextOfYears"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Yıllar için yerel metni alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofyears/
---
## PivotGlobalizationSettings.GetTextOfYears method

"Years" ifadesinin yerel metnini alır.

```csharp
public virtual string GetTextOfYears()
```

### Örnekler

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
            // Özel küreselleşme ayarları oluşturun
            var customSettings = new CustomPivotGlobalizationSettings();
            
            // GetTextOfYears yöntemini göster
            Console.WriteLine("Custom Text of Years: " + customSettings.GetTextOfYears());
        }
    }

    public class CustomPivotGlobalizationSettings : PivotGlobalizationSettings
    {
        public override string GetTextOfYears()
        {
            // \"Years\" etiketi için özel metin döndür
            return "Custom Years Label";
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


