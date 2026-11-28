---
title: "ConditionalFormattingValue.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingValue özelliği. Bu koşullu biçimlendirme değer nesnesinin değerini alın veya ayarlayın. Type ile birlikte kullanılmalıdır."
type: docs
url: /tr/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

Bu koşullu biçimlendirme değer nesnesinin değerini alın veya ayarlayın. Tip ile birlikte kullanılmalıdır.

```csharp
public object Value { get; set; }
```

### Açıklamalar

Değer bir dize ise ve "=" ile başlıyorsa, formül olarak işlenecek, aksi takdirde basit bir değer olarak işlenecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
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
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // Simge seti koşullu biçimlendirmesi oluştur
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // Koşullu biçimlendirme değer nesnelerini alın
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // Simgeler için değerleri ayarlayın
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // Value özelliğinin kullanımını gösterin
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


