---
title: "PivotOptions sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Charts.PivotOptions sınıfı. Grafik üzerinde görünen pivot denetimlerini belirten karmaşık bir türü temsil eder."
type: docs
url: /tr/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Grafikte görünen pivot kontrollerini belirten karmaşık bir türü temsil eder.

```csharp
public class PivotOptions
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın satır eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın veri eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın sayfa eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | dropZonesVisible true olarak ayarlandığında, kaynak PivotTable'ın sütun eksenindeki her PivotTable alanı için bir denetimin grafikte görünüp görünmeyeceğini belirtir. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Pivot grafiğinde herhangi bir pivot denetiminin görünüp görünmeyeceğini belirtir. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Genişletme veya daraltma alan düğmelerinin gösterilip gösterilmeyeceğini belirten bir değeri alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pivot tablo için bazı veriler ekleyin.
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Bir pivot tablo ekle
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Bir grafik ekleyin
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Grafiğin PivotOptions'ına erişin.
            PivotOptions pivotOptions = chart.PivotOptions;

            // PivotOptions özelliklerini ayarlayın.
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Çalışma kitabını kaydedin
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


