---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingValue özelliği. Greater Than Or Equal bayrağını alın veya ayarlayın. Yalnızca ikon setleri için kullanılır ve bu eşik değerinin büyük eşit operatörünü kullanıp kullanmadığını belirler. false, büyük eşit yerine sadece büyük kullanıldığını gösterir. Varsayılan değer true'tir."
type: docs
url: /tr/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Büyük veya Eşit bayrağını alın veya ayarlayın. Yalnızca ikon setleri için kullanın, bu eşik değerinin büyük veya eşit operatörünü kullanıp kullanmadığını belirler. 'false' değeri, 'büyük veya eşit' yerine 'büyük' kullanıldığını gösterir. Varsayılan değer true'tır.

```csharp
public bool IsGTE { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Koşullu biçimlendirme ekle
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Renk ölçeği biçimi oluşturun
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // 2 renkli ölçeği yapılandırın
            fc.ColorScale.Is3ColorScale = false;
            
            // Maksimum değer biçimini ayarlayın (IsGTE gösterimiyle)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Minimum değer biçimini ayarlayın
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Çalışma kitabını kaydedin
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


