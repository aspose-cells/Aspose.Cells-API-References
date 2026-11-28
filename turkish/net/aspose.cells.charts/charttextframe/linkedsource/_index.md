---
title: "ChartTextFrame.LinkedSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ChartTextFrame özelliği. Çalışma sayfasına bir referans alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Çalışma sayfasına bir referansı alır ve ayarlar.

```csharp
public virtual string LinkedSource { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veri ekleyin.
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // Grafik ekle
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Grafik başlığını ayarla ve P1 hücresine bağla
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Bağlantılı kaynağı doğrulayın
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### Ayrıca Bakınız

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


