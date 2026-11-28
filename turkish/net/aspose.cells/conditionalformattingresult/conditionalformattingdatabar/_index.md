---
title: "ConditionalFormattingResult.ConditionalFormattingDataBar"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingResult özelliği. DataBar nesnesini alır."
type: docs
url: /tr/net/aspose.cells/conditionalformattingresult/conditionalformattingdatabar/
---
## ConditionalFormattingResult.ConditionalFormattingDataBar property

DataBar nesnesini alır.

```csharp
public DataBar ConditionalFormattingDataBar { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingResultPropertyConditionalFormattingDataBarDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek değerler ekleyin.
            worksheet.Cells["A1"].PutValue(-6);
            worksheet.Cells["A2"].PutValue(-4);
            worksheet.Cells["A3"].PutValue(-2);
            worksheet.Cells["A4"].PutValue(0);
            worksheet.Cells["A5"].PutValue(2);
            worksheet.Cells["A6"].PutValue(4);
            worksheet.Cells["A7"].PutValue(6);

            // Veri çubuğu koşullu biçimlendirmesi ekle
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 6;
            area.EndColumn = 0;
            fcc.AddArea(area);

            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition condition = fcc[conditionIndex];
            condition.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            condition.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            condition.DataBar.Color = System.Drawing.Color.Green;

            // Formülleri hesaplayın ve biçimlendirmeyi uygulayın.
            workbook.CalculateFormula();

            // Koşullu biçimlendirme sonucunu alın ve DataBar özelliklerini gösterin.
            Cell cell = worksheet.Cells["A1"];
            ConditionalFormattingResult formattingResult = cell.GetConditionalFormattingResult();
            
            Console.WriteLine("DataBar Min Value: " + formattingResult.ConditionalFormattingDataBar.MinCfvo.Value);
            Console.WriteLine("DataBar Max Value: " + formattingResult.ConditionalFormattingDataBar.MaxCfvo.Value);
            Console.WriteLine("DataBar Color: " + formattingResult.ConditionalFormattingDataBar.Color);
        }
    }
}
```

### Ayrıca Bakınız

* class [DataBar](../../databar/)
* class [ConditionalFormattingResult](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


