---
title: "WorkbookSettings.AutoRecover"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/autorecover/
---
## WorkbookSettings.AutoRecover property

Dosyanın otomatik kurtarma için işaretlenip işaretlenmediğini gösterir.

```csharp
public bool AutoRecover { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAutoRecoverDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // AutoRecover ve diğer ayarları yap
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;

            // Çalışma kitabını kaydedin
            string outputPath = "WorkbookSettings_AutoRecoverDemo.xlsx";
            workbook.Save(outputPath);

            // Ayarları doğrulamak için kaydedilmiş çalışma kitabını yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            
            // Ayarları konsola yazdır
            Console.WriteLine("AutoRecover: " + loadedWorkbook.Settings.AutoRecover);
            Console.WriteLine("DataExtractLoad: " + loadedWorkbook.Settings.DataExtractLoad);
            Console.WriteLine("CrashSave: " + loadedWorkbook.Settings.CrashSave);
            Console.WriteLine("RepairLoad: " + loadedWorkbook.Settings.RepairLoad);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


