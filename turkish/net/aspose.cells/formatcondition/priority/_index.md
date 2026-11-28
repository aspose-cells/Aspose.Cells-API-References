---
title: "FormatCondition.Priority"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçimin değerlendirileceğini ve işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir; 1 en yüksek önceliktir."
type: docs
url: /tr/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

Bu koşullu biçimlendirme kuralının önceliği. Bu değer, hangi biçimin değerlendirileceğini ve işleneceğini belirlemek için kullanılır. Daha düşük sayısal değerler, daha yüksek sayısal değerlerden daha yüksek önceliğe sahiptir; '1' en yüksek önceliği temsil eder.

```csharp
public int Priority { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // Koşullu biçimlendirme ekle
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // Koşullar ekle
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // Öncelikleri ayarla
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // Priority özelliğinin kullanımını göster
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // Çalışma kitabını kaydedin
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


