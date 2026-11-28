---
title: "Enum DataBarNegativeColorType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBarNegativeColorType enum. Pozitif veri çubuklarıyla aynı kenarlık ve doldurma renginin kullanılıp kullanılmayacağını belirtir"
type: docs
url: /tr/net/aspose.cells/databarnegativecolortype/
---
## DataBarNegativeColorType enumeration

Pozitif veri çubuklarıyla aynı kenarlık ve dolgu renginin kullanılıp kullanılmayacağını belirtir.

```csharp
public enum DataBarNegativeColorType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Color | `0` | Negatif Değer ve Eksen Ayarı iletişim kutusunda belirtilen rengi veya NegativeBarFormat nesnesinin ColorType ve BorderColorType özelliklerini kullanarak rengi kullanın. |
| SameAsPositive | `1` | Pozitif veri çubuklarıyla aynı rengi kullan. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataBarNegativeColorTypeDemo
    {
        public static void DataBarNegativeColorTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(-20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(-40);
            worksheet.Cells["A5"].PutValue(50);

            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // Veri çubuğu özelliklerini ayarla
            DataBar dataBar = fc.DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Number;
            dataBar.MinCfvo.Value = -50;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Number;
            dataBar.MaxCfvo.Value = 50;
            dataBar.Color = System.Drawing.Color.Green;

            // Negatif çubuk biçim özelliklerini ayarla
            NegativeBarFormat negativeBarFormat = dataBar.NegativeBarFormat;
            negativeBarFormat.Color = System.Drawing.Color.Red;
            negativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            negativeBarFormat.BorderColor = System.Drawing.Color.Blue;
            negativeBarFormat.BorderColorType = DataBarNegativeColorType.SameAsPositive;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarNegativeColorTypeExample.xlsx");
            workbook.Save("DataBarNegativeColorTypeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


