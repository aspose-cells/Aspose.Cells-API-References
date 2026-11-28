---
title: "FormatCondition.StopIfTrue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. True olduğunda, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz. Yalnızca Excel 2007 için geçerlidir."
type: docs
url: /tr/net/aspose.cells/formatcondition/stopiftrue/
---
## FormatCondition.StopIfTrue property

Doğru, bu kural doğru değerlendirildiğinde, daha düşük öncelikli kurallar bu kuralın üzerine uygulanamaz. Yalnızca Excel 2007 için geçerlidir;

```csharp
public bool StopIfTrue { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStopIfTrueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Koşullu biçimlendirme ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
            // Koşul ekle ve StopIfTrue'ı ayarla
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "15", "35");
            FormatCondition condition = fcs[conditionIndex];
            condition.StopIfTrue = true;
            
            // Normalde birincisini geçersiz kılan başka bir koşul ekle
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "25", "");
            FormatCondition condition2 = fcs[conditionIndex2];
            condition2.StopIfTrue = false;

            // Çalışma kitabını kaydedin
            workbook.Save("StopIfTrueDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


