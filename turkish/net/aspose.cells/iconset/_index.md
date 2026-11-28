---
title: "Sınıf IconSet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.IconSet sınıfı. IconSet koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, ikonları hücrelerin değerlerine göre uygular."
type: docs
url: /tr/net/aspose.cells/iconset/
---
## IconSet class

IconSet koşullu biçimlendirme kuralını açıklar. Bu koşullu biçimlendirme kuralı, hücrelere değerlerine göre simgeler uygular.

```csharp
public class IconSet
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | Koleksiyondan [`ConditionalFormattingIcon`](../conditionalformattingicon/) alın |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | CFValueObjects örneğini alın. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | İkon setinin özelleştirilmiş olup olmadığını gösterir. Varsayılan değer false'tur. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | Bu ikon setindeki ikonların varsayılan sırasını tersine çevirip çevirmediğini gösteren bayrağı alın veya ayarlayın. Varsayılan değer false'tur. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | Bu ikon setinin uygulandığı hücrelerin değerlerini gösterip göstermediğini belirten bayrağı alın veya ayarlayın. Varsayılan değer true'dur. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | Görüntülenecek ikon seti türünü alın veya ayarlayın. Tür ayarlandığında, mevcut Cfvos sayısının yeni türle uyumlu olup olmadığı otomatik olarak kontrol edilir. Uyumsuzsa, eski Cfvos temizlenir ve varsayılan Cfvos eklenir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Koşul ekler
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // İkon setini al
            IconSet iconSet = cond.IconSet;

            // İkon tipini ayarla
            iconSet.Type = IconSetType.Arrows3;

            // Ek özellikleri ayarla
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Hücre değerlerini yerleştir
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Excel dosyasını kaydetme
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


