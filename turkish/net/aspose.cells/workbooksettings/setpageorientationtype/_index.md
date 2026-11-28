---
title: "WorkbookSettings.SetPageOrientationType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings yöntemi. Tüm çalışma kitabı için baskı yönlendirme tipini ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/setpageorientationtype/
---
## WorkbookSettings.SetPageOrientationType method

Tüm çalışma kitabı için baskı yönlendirme tipini ayarlar.

```csharp
public void SetPageOrientationType(PageOrientationType pageOrientationType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageOrientationType | PageOrientationType | Sayfa yönlendirme tipi |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsMethodSetPageOrientationTypeWithPageOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();
            
            // Tüm çalışma sayfaları için sayfa yönlendirmesini Dikey (Portrait) olarak ayarlayın
            workbook.Settings.SetPageOrientationType(PageOrientationType.Portrait);
            
            // Yönlendirmenin doğru ayarlandığını doğrulayın
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine("Worksheet: " + sheet.Name + " - Orientation: " + sheet.PageSetup.Orientation);
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [PageOrientationType](../../pageorientationtype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


