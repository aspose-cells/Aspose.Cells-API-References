---
title: "FormatCondition.TimePeriod"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Tarih içinde gerçekleşen bir koşullu biçimlendirme kuralında uygulanabilir zaman dilimi. Yalnızca timePeriod türü için geçerlidir. Varsayılan değer TimePeriodType.Today'dir."
type: docs
url: /tr/net/aspose.cells/formatcondition/timeperiod/
---
## FormatCondition.TimePeriod property

"date occurrin" koşullu biçimlendirme kuralındaki uygulanabilir zaman dilimidir. Yalnızca type = timePeriod için geçerlidir. Varsayılan değer TimePeriodType.Today'dir.

```csharp
public TimePeriodType TimePeriod { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTimePeriodDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zaman dilimi biçimlendirmesini göstermek için örnek tarih değerleri ekleyin
            worksheet.Cells["A1"].PutValue(DateTime.Now);
            worksheet.Cells["A2"].PutValue(DateTime.Now.AddDays(-1));
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));

            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            int conditionIndex = fcs.AddCondition(FormatConditionType.TimePeriod);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.LightBlue;
            fc.TimePeriod = TimePeriodType.Today;

            workbook.Save("TimePeriodDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TimePeriodType](../../timeperiodtype/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


