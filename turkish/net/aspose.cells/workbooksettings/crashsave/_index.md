---
title: "WorkbookSettings.CrashSave"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

Uygulamanın çöküşten sonra çalışma kitabı dosyasını en son kaydedip kaydetmediğini gösterir.

```csharp
public bool CrashSave { get; set; }
```

### Örnekler

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // Çalışma kitabı ayarlarına eriş
            WorkbookSettings settings = workbook.Settings;

            // CrashSave özelliğini göster
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Çöküş kaydetme etkinleştirildiğinde kaydet
            workbook.Save("CrashSaveEnabled.xlsx");

            // Çöküş kaydetmeyi devre dışı bırak
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // Çöküş kaydetme devre dışı bırakıldığında kaydet
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


