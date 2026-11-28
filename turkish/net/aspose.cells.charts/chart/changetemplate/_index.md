---
title: "Chart.ChangeTemplate"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Chart yöntemi. Önceden ayarlanmış bir şablonla grafik tipini değiştir"
type: docs
url: /tr/net/aspose.cells.charts/chart/changetemplate/
---
## Chart.ChangeTemplate method

Önceden ayarlanmış bir şablonla grafik tipini değiştir.

```csharp
public void ChangeTemplate(byte[] data)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| veri | Byte[] | Grafik şablon dosyasının (.crtx) verileri. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.IO;

    public class ChartMethodChangeTemplateWithByteDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Grafik veri aralığını ayarla
            chart.SetChartDataRange("A1:B4", false);

            // Başka bir grafik dosyasından şablon verilerini al
            byte[] templateData = File.ReadAllBytes("ChartTemplate.crtx");

            try
            {
                // ChangeTemplate yöntemini bayt dizisi parametresiyle çağır
                chart.ChangeTemplate(templateData);
                
                Console.WriteLine("Chart template changed successfully using byte array parameter");
                
                // Çalışma kitabını kaydederek etkiyi göster
                workbook.Save("ChartWithChangedTemplate.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error changing chart template: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


