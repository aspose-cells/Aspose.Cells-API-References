---
title: "WorkbookSettings.MemorySetting"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bellek kullanım seçeneklerini alır veya ayarlar. Yeni seçenek, yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınacak, ancak mevcut çalışma sayfaları için etkili olmayacaktır."
type: docs
url: /tr/net/aspose.cells/workbooksettings/memorysetting/
---
## WorkbookSettings.MemorySetting property

Bellek kullanımı seçeneklerini alır veya ayarlar. Yeni seçenek, yeni oluşturulan çalışma sayfaları için varsayılan seçenek olarak alınır ancak mevcut çalışma sayfaları için etkili olmaz.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### Açıklamalar

Bellek modu hakkında daha fazla ayrıntı için lütfen [`MemorySetting`](../../cells/memorysetting/) adresine bakın.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // Bellek tercih ayarıyla yeni bir çalışma kitabı oluşturun
            Workbook wb = new Workbook();
            wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
            
            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet sheet = wb.Worksheets[0];
            sheet.Cells["A1"].PutValue("Memory Setting Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // PDF formatında bellek akışına kaydedin
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Pdf);
                Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


