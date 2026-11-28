---
title: "DataBar.MaxCfvo"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataBar özelliği. Bu DataBar'ın maksimum değer nesnesini alır veya ayarlar. Boş (null) veya FormatConditionValueType.Min tipinde CFValueObject atanamaz"
type: docs
url: /tr/net/aspose.cells/databar/maxcfvo/
---
## DataBar.MaxCfvo property

Bu DataBar'ın maksimum değer nesnesini al veya ayarla. Null veya FormatConditionValueType.Min tipinde CFValueObject'i ona atayamazsınız.

```csharp
public ConditionalFormattingValue MaxCfvo { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataBarPropertyMaxCfvoDemo
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

            // Veri çubuğu koşullu biçimlendirmesi ekle
            int idx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Veri çubuğu ekle
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            DataBar dataBar = fcc[conditionIndex].DataBar;

            // MaxCfvo değerini ayarla
            dataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            dataBar.MaxCfvo.Value = 50;

            // Çalışma kitabını kaydedin
            workbook.Save("DataBarMaxCfvoDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


