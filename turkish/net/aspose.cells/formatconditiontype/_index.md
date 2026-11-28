---
title: "Enum FormatConditionType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.FormatConditionType enum. Koşullu biçim kuralı türü"
type: docs
url: /tr/net/aspose.cells/formatconditiontype/
---
## FormatConditionType enumeration

Koşullu biçim kuralı türü.

```csharp
public enum FormatConditionType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| CellValue | `1` | Bu koşullu biçimlendirme kuralı, bir hücre değerini bir formülün hesaplanan sonucu ile bir operatör kullanarak karşılaştırır. |
| Expression | `2` | Bu koşullu biçimlendirme kuralı, değerlendirilmesi gereken bir formül içerir. Formül sonucu doğru olduğunda, hücre vurgulanır. |
| Top10 | `4` | Bu koşullu biçimlendirme kuralı, belirtilen şekilde değerleri üst N veya alt N aralığına düşen hücreleri vurgular. |
| UniqueValues | `8` | Bu koşullu biçimlendirme kuralı, aralıktaki benzersiz değerleri vurgular. |
| DuplicateValues | `16` | Bu koşullu biçimlendirme kuralı, yinelenen değerleri vurgular. |
| ContainsText | `32` | Bu koşullu biçimlendirme kuralı, verilen metni içeren hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevinin kullanılmasına eşdeğerdir. |
| NotContainsText | `64` | Bu koşullu biçimlendirme kuralı, verilen metni içermeyen hücreleri vurgular. Hücrenin metni içerip içermediğini belirlemek için SEARCH() sayfa işlevinin kullanılmasına eşdeğerdir. |
| BeginsWith | `128` | Bu koşullu biçimlendirme kuralı, verilen metinle başlayan hücreleri aralıkta vurgular. LEFT() sayfa işlevinin kullanılması ve değerlerin karşılaştırılmasıyla eşdeğerdir. |
| EndsWith | `256` | Bu koşullu biçimlendirme kuralı, verilen metinle biten hücreleri vurgular. RIGHT() sayfa işlevinin kullanılması ve değerlerin karşılaştırılmasıyla eşdeğerdir. |
| ContainsBlanks | `512` | Bu koşullu biçimlendirme kuralı, tamamen boş olan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| NotContainsBlanks | `1024` | Bu koşullu biçimlendirme kuralı, boş olmayan hücreleri vurgular. LEN(TRIM()) kullanımına eşdeğerdir. Bu, hücre yalnızca TRIM()'in kaldıracağı karakterleri içeriyorsa boş olarak kabul edildiği anlamına gelir. Boş bir hücre de boş olarak kabul edilir. |
| ContainsErrors | `2048` | Bu koşullu biçimlendirme kuralı, formül hatası olan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevinin kullanılmasına eşdeğerdir. |
| NotContainsErrors | `4096` | Bu koşullu biçimlendirme kuralı, formül hatası olmayan hücreleri vurgular. Formül hatası olup olmadığını belirlemek için ISERROR() sayfa işlevinin kullanılmasına eşdeğerdir. |
| TimePeriod | `8192` | Bu koşullu biçimlendirme kuralı, belirtilen zaman dilimindeki tarihleri içeren hücreleri vurgular. Hücrenin temel değeri değerlendirilir, bu nedenle hücrenin tarih olarak biçimlendirilmiş olması değerlendirme için gerekli değildir. Örneğin, değeri 38913 olan bir hücrede, kural 7/14/2006 tarihini gerektiriyorsa koşullu biçimlendirme uygulanır. |
| AboveAverage | `16384` | Bu koşullu biçimlendirme kuralı, aralıktaki tüm değerlerin ortalamasının üzerindeki veya altındaki hücreleri vurgular. |
| ColorScale | `32768` | Bu koşullu biçimlendirme kuralı, hücrelerde kademeli bir renk ölçeği oluşturur. |
| DataBar | `65536` | Bu koşullu biçimlendirme kuralı, hücre aralığında kademeli bir veri çubuğu gösterir. |
| IconSet | `131072` | Bu koşullu biçimlendirme kuralı, hücreleri değerlerine göre simgelerle işaretler. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FormatConditionTypeDemo
    {
        public static void FormatConditionTypeExample()
        {
            // Yeni bir Workbook oluştur.
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasını al.
            Worksheet worksheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 10
            };
            fcs.AddArea(ca);

            // AboveAverage için bir koşul ekler
            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Yellow;

            // AboveAverage için özellikleri ayarlama
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // CellValue için bir koşul ekler
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = Color.Red;

            // ContainsText için bir koşul ekler
            int conditionIndex3 = fcs.AddCondition(FormatConditionType.ContainsText);
            FormatCondition fc3 = fcs[conditionIndex3];
            fc3.Text = "Sample";
            fc3.Style.BackgroundColor = Color.Green;

            // Excel dosyasını kaydet
            workbook.Save("FormatConditionTypeExample.xlsx");
            workbook.Save("FormatConditionTypeExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


