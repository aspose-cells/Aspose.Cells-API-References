---
title: "WorkbookSettings.FirstVisibleTab"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Görünür ilk çalışma sayfası sekmesini alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/workbooksettings/firstvisibletab/
---
## WorkbookSettings.FirstVisibleTab property

İlk görünen çalışma sayfası sekmesini alır veya ayarlar.

```csharp
public int FirstVisibleTab { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyFirstVisibleTabDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            workbook.Worksheets.Add("Sheet1");
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // İlk görünür sekme indeksini ayarla (0 tabanlı)
            workbook.Settings.FirstVisibleTab = 1;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
            
            // Ayarı doğrula
            Console.WriteLine("First visible tab index: " + workbook.Settings.FirstVisibleTab);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


