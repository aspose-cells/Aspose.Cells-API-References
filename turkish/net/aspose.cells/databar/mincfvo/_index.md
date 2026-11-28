---
title: "DataBar.MinCfvo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Bu DataBar'ın minimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Max tipinde CFValueObject atanamaz"
type: docs
url: /tr/net/aspose.cells/databar/mincfvo/
---
## DataBar.MinCfvo property

Bu DataBar'ın minimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Max tipinde CFValueObject'i ona atayamazsınız.

```csharp
public ConditionalFormattingValue MinCfvo { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMinCfvoDemo
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

            // Koşullu biçimlendirme koleksiyonunu alın
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];

            // MinCfvo "Value" türüne ayarlanmış bir veri çubuğu oluştur
            fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[0].DataBar;
            dataBar.MinCfvo.Type = FormatConditionValueType.Min;
            dataBar.MinCfvo.Value = "5"; // Minimum value for the data bar

            // Veri çubuğu aralığını ayarla
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 3;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarMinCfvoDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


