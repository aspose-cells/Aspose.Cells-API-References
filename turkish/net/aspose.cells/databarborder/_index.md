---
title: "Sınıf DataBarBorder"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBarBorder sınıfı. Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenarlığını temsil eder"
type: docs
url: /tr/net/aspose.cells/databarborder/
---
## DataBarBorder class

Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenarlığını temsil eder.

```csharp
public class DataBarBorder
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenarlık rengini alır veya ayarlar. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | Koşullu biçimlendirme kuralı tarafından belirtilen veri çubuklarının kenarlık tipini alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // Yeni bir çalışma kitabı oluşturma
            Workbook workbook = new Workbook();
            // Çalışma kitabındaki ilk çalışma sayfasına erişme
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bazı örnek veriler ekleme
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // Boş bir koşullu biçimlendirme ekleme
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme için hücre alanı tanımlama
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // DataBar türünde bir koşul ekleme
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // DataBar'a erişme
            DataBar dataBar = formatCondition.DataBar;

            // DataBar özelliklerini ayarlama
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // DataBarBorder özelliklerine erişme ve ayarlama
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // Excel dosyasını kaydetme
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


