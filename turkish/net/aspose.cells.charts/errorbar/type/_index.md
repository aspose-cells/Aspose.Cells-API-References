---
title: "ErrorBar.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ErrorBar özelliği. Hata çubuğu miktar türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Hata çubuğu miktar tipini temsil eder.

```csharp
public ErrorBarType Type { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Örnek veri ekleyin.
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Bir grafik oluştur
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Seri verisi ekle
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Özel hata çubuğu türünü ve değerlerini ayarla
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Çalışma kitabını kaydedin
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


