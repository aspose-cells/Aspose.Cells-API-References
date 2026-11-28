---
title: "DataBar.BarFillType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Bir veri çubuğunun renkle nasıl doldurulacağını alır veya ayarlar"
type: docs
url: /tr/net/aspose.cells/databar/barfilltype/
---
## DataBar.BarFillType property

Bir veri çubuğunun renkle nasıl doldurulacağını alır veya ayarlar.

```csharp
public DataBarFillType BarFillType { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyBarFillTypeDemo
    {
        public static void Run()
        {
            // Bir Workbook nesnesi oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarla
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 5,
                StartColumn = 0,
                EndColumn = 5
            };
            fcs.AddArea(ca);

            // DataBar koşulu ekle
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcs[conditionIndex];

            // DataBar özelliklerini yapılandır
            DataBar dataBar = fc.DataBar;
            dataBar.BarFillType = DataBarFillType.Gradient; // Demonstrating BarFillType usage
            dataBar.Color = Color.Blue;

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(100);

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarFillTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [DataBarFillType](../../databarfilltype/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


