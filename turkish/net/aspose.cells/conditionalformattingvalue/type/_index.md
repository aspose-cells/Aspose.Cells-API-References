---
title: "ConditionalFormattingValue.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingValue özelliği. Bu koşullu biçimlendirme değer nesnesinin tipini alın veya ayarlayın. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, Value'yu otomatik olarak null yapar."
type: docs
url: /tr/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

Bu koşullu biçimlendirme değer nesnesinin tipini alın veya ayarlayın. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, "Value" değerini otomatik olarak null yapar.

```csharp
public FormatConditionValueType Type { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // Bazı örnek veriler ekleyin (koşullu biçimlendirmenin mevcut olması için gereklidir)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // Bir koşullu biçimlendirme koleksiyonu oluşturun ve bir IconSet koşulu ekleyin
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // IconSet koleksiyonundan bir ConditionalFormattingValue örneği alın
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // Type'ı Percent olarak ayarlayın ve ilgili bir değer atayın
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // Type ve Value'yu okuyun ve gösterin
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // Type'ı Min olarak değiştirin – belgelerde belirtildiği gibi bu, Value'yu null yapar
                cfv.Type = FormatConditionValueType.Min;

                // Type ve Value'yu tekrar okuyun ve gösterin
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // Çalışma kitabını kaydedin (koşullu biçimlendirme sayfanın bir parçasıdır)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


