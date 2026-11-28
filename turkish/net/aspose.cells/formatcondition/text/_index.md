---
title: "FormatCondition.Text"
second_title: "Aspose.Cells için .NET API Referansı"
description: "FormatCondition özelliği. Metin değerinin bir metin içinde koşullu biçimlendirme kuralı içerdiği. Yalnızca containsText, notContainsText, beginsWith ve endsWith türleri için geçerlidir. Varsayılan değer null'dur."
type: docs
url: /tr/net/aspose.cells/formatcondition/text/
---
## FormatCondition.Text property

"text contains" koşullu biçimlendirme kuralındaki metin değeridir. Yalnızca type = containsText, notContainsText, beginsWith ve endsWith için geçerlidir. Varsayılan değer null'dur.

```csharp
public string Text { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyTextDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Koşullu biçimlendirme ekle
            ConditionalFormattingCollection conditionalFormattings = sheet.ConditionalFormattings;
            int collectionIndex = conditionalFormattings.Add();
            FormatConditionCollection formatConditions = conditionalFormattings[collectionIndex];

            // Metin koşulu ekle
            int conditionIndex = formatConditions.AddCondition(FormatConditionType.ContainsText);
            FormatCondition formatCondition = formatConditions[conditionIndex];
            
            // Metin özelliğini ayarlayın (Rusça metin gösterimi)
            formatCondition.Text = "вс";

            // Biçimlendirme stilini uygulayın
            Style style = formatCondition.Style;
            style.BackgroundColor = Color.Red;
            formatCondition.Style = style;

            // A1 hücresine uygula
            formatConditions.AddArea(CellArea.CreateCellArea("A1", "A1"));

            // Kaydet ve doğrula
            string outputPath = "FormatConditionPropertyTextDemo_Output.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("FormatCondition Text property demo completed successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


