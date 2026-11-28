---
title: "Chart.RefreshPivotData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart metodu. Grafik verilerini pivot tablo üzerinden yeniler"
type: docs
url: /tr/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Grafiğin verilerini özet tablodan yeniler.

```csharp
public void RefreshPivotData()
```

### Açıklamalar

Pivot veri kaynağından pivot tablo raporuna veri toplayacağız. Bu metod yalnızca tüm verileri bir pivot grafik için toplamak amacıyla kullanılır.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına örnek veri ekle
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Bir pivot tablo oluştur
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Bir grafik ekleyin
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Pivot grafik veri kaynağını ayarla
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Grafikteki pivot verilerini yenile
            chart.RefreshPivotData();
            
            // Çalışma kitabını kaydedin
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


