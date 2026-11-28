---
title: "Enum DataLabelsSeparatorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.DataLabelsSeparatorType enum. DataLabels ayırıcı tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

DataLabels ayırıcı tipini temsil eder.

```csharp
public enum DataLabelsSeparatorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Auto | `0` | Otomatik ayırıcıyı temsil eder |
| Space | `1` | Boşluk (" ") temsil eder |
| Comma | `2` | Virgül (",") temsil eder |
| Semicolon | `3` | Noktalı virgül (";") temsil eder |
| Period | `4` | Nokta (".") temsil eder |
| NewLine | `5` | Yeni satır ("\n") temsil eder |
| Custom | `6` | Özel ayırıcıyı temsil eder |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Grafik için bazı veriler ekleyin
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Çalışma sayfasına bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Veri serisini grafiğe ekle
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // İlk serinin veri etiketlerine eriş
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Ayırıcı türünü virgül olarak ayarlayın
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Veri etiketlerini etkinleştirin ve bazı özellikleri ayarlayın
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Yazı tipi özelliklerini ayarlayın
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Çalışma kitabını kaydedin
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


