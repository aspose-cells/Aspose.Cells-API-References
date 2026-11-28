---
title: "Sınıf NegativeBarFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.NegativeBarFormat sınıfı. Veri çubuğu koşullu biçimlendirme kuralı tarafından tanımlanan negatif değerler için veri çubuklarının renk ayarlarını temsil eder."
type: docs
url: /tr/net/aspose.cells/negativebarformat/
---
## NegativeBarFormat class

Koşullu biçimlendirme kuralı tarafından tanımlanan negatif değerler için veri çubuklarının renk ayarlarını temsil eder.

```csharp
public class NegativeBarFormat
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [BorderColor](../../aspose.cells/negativebarformat/bordercolor/) { get; set; } | Negatif veri çubukları için kenar rengi belirlemek amacıyla kullanabileceğiniz bir FormatColor nesnesini alır veya ayarlar. |
| [BorderColorType](../../aspose.cells/negativebarformat/bordercolortype/) { get; set; } | Pozitif veri çubuklarıyla aynı kenar renginin kullanılıp kullanılmayacağını gösterir. |
| [Color](../../aspose.cells/negativebarformat/color/) { get; set; } | Negatif veri çubukları için dolgu rengi belirlemek amacıyla kullanabileceğiniz bir FormatColor nesnesini alır veya ayarlar. |
| [ColorType](../../aspose.cells/negativebarformat/colortype/) { get; set; } | Pozitif veri çubuklarıyla aynı dolgu renginin kullanılıp kullanılmayacağını alır veya ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class NegativeBarFormatDemo
    {
        public static void NegativeBarFormatExample()
        {
            // Bir Workbook nesnesi oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // DataBar için koşul ekler
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // DataBar'ı al ve özelliklerini ayarla
            DataBar dataBar = fc.DataBar;
            dataBar.Color = Color.Orange;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;

            // NegativeBarFormat özelliklerini yapılandır
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = Color.White;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = Color.Yellow;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;

            // Hücrelere bazı değerler koyun
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(120);
            worksheet.Cells["A3"].PutValue(260);

            // Çalışma kitabını kaydedin
            workbook.Save("NegativeBarFormatExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


