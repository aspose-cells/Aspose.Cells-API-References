---
title: "ConditionalFormattingCollection.Copy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ConditionalFormattingCollection yöntemi. Koşullu biçimlendirmeyi kopyalar"
type: docs
url: /tr/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Koşullu biçimlendirmeyi kopyalar.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | Koşullu biçimlendirme |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Koşullu biçimlendirme içeren bir kaynak çalışma kitabı oluşturun
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Kaynak sayfaya örnek koşullu biçimlendirme ekleyin
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Biçim koşuluna stil oluşturun ve uygulayın
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Bir aralığa uygulayın
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Koşullu biçimlendirmeyi kaynaktan hedefe kopyalayın
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Çalışma kitabını kaydedin
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


