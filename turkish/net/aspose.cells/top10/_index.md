---
title: "Sınıf Top10"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Top10 sınıfı. Top10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, değerleri belirtilen üst N veya alt N aralığına düşen hücreleri vurgular"
type: docs
url: /tr/net/aspose.cells/top10/
---
## Top10 class

Top10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, değerleri belirtilen şekilde en üst N veya en alt N aralığına düşen hücreleri vurgular.

```csharp
public class Top10
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Top10](top10/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | \"top/bottom n\" kuralının \"bottom n\" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | \"top/bottom n\" kuralının \"top/bottom n percent\" kuralı olup olmadığını alın veya ayarlayın. Varsayılan değer false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | \"top/bottom n\" koşullu biçimlendirme kuralında \"n\" değerini alın veya ayarlayın. IsPercent true ise değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class Top10Demo
    {
        public static void Top10Example()
        {
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Boş bir koşullu biçimlendirme ekler
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Koşullu biçimlendirme aralığını ayarlar
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // Koşul ekler
            int conditionIndex = fcs.AddCondition(FormatConditionType.Top10);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = Color.Red;

            // Özellikleri ayarlama
            Top10 top10 = fc.Top10;
            top10.IsPercent = false;
            top10.IsBottom = false;
            top10.Rank = 5;

            // Excel dosyasını kaydetme
            workbook.Save("Top10Example.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


