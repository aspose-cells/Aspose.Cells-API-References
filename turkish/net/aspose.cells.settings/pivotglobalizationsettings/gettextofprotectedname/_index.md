---
title: "PivotGlobalizationSettings.GetTextOfProtectedName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PivotGlobalizationSettings yöntemi. Belirtilen korumalı ad için metni alır"
type: docs
url: /tr/net/aspose.cells.settings/pivotglobalizationsettings/gettextofprotectedname/
---
## PivotGlobalizationSettings.GetTextOfProtectedName method

Belirtilen korumalı ad için metni alır.

```csharp
public virtual string GetTextOfProtectedName(string protectedName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| protectedName | String | PivotTable'daki korumalı ad. |

### Dönüş Değeri

PivotTable'ın yerel korumalı adları.

### Açıklamalar

Ms Excel'de, bazı adların PivotTable'da PivotFields adı olarak kullanılması izin verilmez. Bunlar bölgeye göre farklılık gösterir, kullanıcı kullanılan bölgeye göre bunları açıkça belirtebilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Settings;

namespace AsposeCellsExamples
{
    public class PivotGlobalizationSettingsMethodGetTextOfProtectedNameWithStringDemo
    {
        public static void Run()
        {
            try
            {
                // PivotGlobalizationSettings örneği oluştur
                PivotGlobalizationSettings globalizationSettings = new PivotGlobalizationSettings();

                // Metnini almak için bir korumalı ad tanımlayın
                string protectedName = "SensitiveData";

                // GetTextOfProtectedName yöntemini çağırın
                string result = globalizationSettings.GetTextOfProtectedName(protectedName);

                // Sonucu çıktı olarak ver
                Console.WriteLine($"Text for protected name \"{protectedName}\": {result}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfProtectedName: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PivotGlobalizationSettings](../)
* namespace [Aspose.Cells.Settings](../../../aspose.cells.settings/)
* assembly [Aspose.Cells](../../../)


