---
title: "Enum DataBarFillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.DataBarFillType enum. Bir veri çubuğunun renkle nasıl doldurulacağını belirtir"
type: docs
url: /tr/net/aspose.cells/databarfilltype/
---
## DataBarFillType enumeration

Bir veri çubuğunun renk ile nasıl doldurulacağını belirtir.

```csharp
public enum DataBarFillType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Solid | `0` | Veri çubuğu katı renk ile doldurulur. |
| Gradient | `1` | Veri çubuğu renk geçişi ile doldurulur. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarFillTypeDemo
    {
        public static void DataBarFillTypeExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();

            // Çalışma Kitabına yeni bir çalışma sayfası ekleniyor
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar.
            CellArea ca = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // Koşul ekler
            int idx = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition cond = fcs[idx];

            // Databar'ı al
            DataBar dataBar = cond.DataBar;

            // Databar özelliklerini ayarla
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 30;
            dataBar.ShowValue = false;
            dataBar.BarBorder.Type = DataBarBorderType.Solid;
            dataBar.BarBorder.Color = Color.Plum;
            dataBar.BarFillType = DataBarFillType.Solid;
            dataBar.AxisColor = Color.Red;
            dataBar.AxisPosition = DataBarAxisPosition.Midpoint;
            dataBar.NegativeBarFormat.ColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.Color = Color.White;
            dataBar.NegativeBarFormat.BorderColorType = DataBarNegativeColorType.Color;
            dataBar.NegativeBarFormat.BorderColor = Color.Yellow;

            // Hücre değerlerini yerleştir
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Excel dosyasını kaydetme
            workbook.Save("DataBarFillTypeExample.xlsx");
            workbook.Save("DataBarFillTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


