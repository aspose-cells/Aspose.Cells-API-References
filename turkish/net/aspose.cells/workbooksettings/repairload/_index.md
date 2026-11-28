---
title: "WorkbookSettings.RepairLoad"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings property. Uygulamanın çalışma kitabını son olarak güvenli ya da onarım modunda açıp açmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/workbooksettings/repairload/
---
## WorkbookSettings.RepairLoad property

Uygulamanın çalışma kitabını en son güvenli ya da onarım modunda açıp açmadığını gösterir.

```csharp
public bool RepairLoad { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyRepairLoadDemo
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
            string outputPath = "WorkbookSettings_RepairLoad_Example.xlsx";
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


