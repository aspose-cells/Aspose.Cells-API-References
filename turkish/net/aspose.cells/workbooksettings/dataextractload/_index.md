---
title: "WorkbookSettings.DataExtractLoad"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Uygulamanın çalışma kitabını son olarak veri kurtarma için açıp açmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/dataextractload/
---
## WorkbookSettings.DataExtractLoad property

Uygulamanın veri kurtarma için çalışma kitabını en son açıp açmadığını gösterir.

```csharp
public bool DataExtractLoad { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDataExtractLoadDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabı ayarlarını yapılandır
            workbook.Settings.AutoRecover = false;
            workbook.Settings.DataExtractLoad = true;
            workbook.Settings.CrashSave = true;
            workbook.Settings.RepairLoad = true;
            
            // Çalışma kitabını kaydedin
            string destPath = "output.xlsx";
            workbook.Save(destPath);
            
            // Ayarları doğrulamak için çalışma kitabını yeniden yükle
            Workbook loadedWorkbook = new Workbook(destPath);
            
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


