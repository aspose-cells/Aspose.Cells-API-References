---
title: "Sınıf ConditionalFormattingIcon"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ConditionalFormattingIcon sınıfı. Koşullu biçimlendirme kuralının özelleştirilmiş ikonunu temsil eder."
type: docs
url: /tr/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

Koşullu biçimlendirme kuralının özel simgesini temsil eder.

```csharp
public class ConditionalFormattingIcon
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | İkon seti verilerini alır. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | İkon setindeki ikonun dizinini alır ve ayarlar. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | İkon seti türünü alır ve ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | Hücrenin ayarıyla görüntü verisini alır. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | İkon seti verisini al |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabındaki ilk çalışma sayfasına erişin
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Koşullu Biçimlendirmeler Koleksiyonu'nu al
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Koleksiyona yeni bir koşullu biçimlendirme ekleyin
            int index = cformattings.Add();
            
            // Biçim Koşulu Koleksiyonuna erişin
            FormatConditionCollection fcs = cformattings[index];
            
            // Koşullu biçimlendirme uygulanacak hücre alanını tanımlayın
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Hücre alanını biçim koşulu koleksiyonuna ekleyin
            fcs.AddArea(ca);
            
            // Simge setlerini kullanmak için bir koşul ekleyin
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Simge seti türünü ayarlayın
            fc.IconSet.Type = IconSetType.Arrows3;

            // Simge seti içindeki bireysel simgeleri özelleştirin
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Çalışma kitabını kaydedin
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


