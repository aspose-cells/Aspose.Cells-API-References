---
title: "WorkbookSettings.PropertiesFollowChartPoint"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookSettings özelliği. Bu çalışma kitabındaki tüm grafiklerde veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir."
type: docs
url: /tr/net/aspose.cells/workbooksettings/propertiesfollowchartpoint/
---
## WorkbookSettings.PropertiesFollowChartPoint property

Bu çalışma kitabındaki tüm grafiklerdeki veri noktası özelliklerinin ve veri etiketlerinin referanslarını takip edip etmediğini gösterir.

```csharp
public bool PropertiesFollowChartPoint { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyPropertiesFollowChartPointDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Grafik için örnek veri ekle
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // PropertiesFollowChartPoint'i true olarak ayarla
            workbook.Settings.PropertiesFollowChartPoint = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Ayarın kaydedildiğini doğrula
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("PropertiesFollowChartPoint: " + loadedWorkbook.Settings.PropertiesFollowChartPoint);
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


