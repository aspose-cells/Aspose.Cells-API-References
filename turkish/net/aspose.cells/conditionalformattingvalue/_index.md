---
title: "Sınıf ConditionalFormattingValue"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ConditionalFormattingValue sınıfı. Bir gradient ölçeği dataBar veya iconSet içindeki ara nokta değerlerini açıklar"
type: docs
url: /tr/net/aspose.cells/conditionalformattingvalue/
---
## ConditionalFormattingValue class

Bir gradient ölçeği, dataBar veya iconSet içindeki ara nokta değerlerini açıklar.

```csharp
public class ConditionalFormattingValue
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsGTE](../../aspose.cells/conditionalformattingvalue/isgte/) { get; set; } | Büyük veya Eşit bayrağını alın veya ayarlayın. Yalnızca ikon setleri için kullanın, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmadığını belirler. 'false' değeri, 'büyük veya eşit' yerine 'büyük' kullanıldığını gösterir. Varsayılan değer true'tır. |
| [Type](../../aspose.cells/conditionalformattingvalue/type/) { get; set; } | Bu koşullu biçimlendirme değer nesnesinin tipini alın veya ayarlayın. Tipi FormatConditionValueType.Min veya FormatConditionValueType.Max olarak ayarlamak, "Value" değerini otomatik olarak null yapar. |
| [Value](../../aspose.cells/conditionalformattingvalue/value/) { get; set; } | Bu koşullu biçimlendirme değer nesnesinin değerini alın veya ayarlayın. Tip ile birlikte kullanılmalıdır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class ConditionalFormattingValueDemo
    {
        public static void ConditionalFormattingValueExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Koşul ekler
            int conditionIndex = fcs.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcs[conditionIndex];

            // ColorScale için özellikleri ayarlama
            fc.ColorScale.Is3ColorScale = true;

            // Minimum değeri ayarlama
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinCfvo.Value = null;
            fc.ColorScale.MinColor = Color.Blue;

            // Orta değeri ayarlama
            fc.ColorScale.MidCfvo.Type = FormatConditionValueType.Percentile;
            fc.ColorScale.MidCfvo.Value = 50;
            fc.ColorScale.MidColor = Color.Yellow;

            // Maksimum değeri ayarlama
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxCfvo.Value = null;
            fc.ColorScale.MaxColor = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("ConditionalFormattingValueExample.xlsx");
            workbook.Save("ConditionalFormattingValueExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


