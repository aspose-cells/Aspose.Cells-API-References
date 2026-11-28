---
title: "Range.Merge"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Hücre aralığını tek bir hücrede birleştirir"
type: docs
url: /tr/net/aspose.cells/range/merge/
---
## Range.Merge method

Bir hücre aralığını tek bir hücreye birleştirir.

```csharp
public void Merge()
```

### Açıklamalar

Birleştirilmiş hücreye, aralıktaki sol üst hücrenin adresi üzerinden başvurun.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMergeDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturun ve hücreleri birleştirin (3 satır x 2 sütun)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            range.Merge();

            // Birleştirilmiş hücrede değeri ayarlayın
            worksheet.Cells[0, 0].Value = "Merged Cells Demo";

            // Birleştirilmiş hücreleri biçimlendirin
            Style style = worksheet.Cells[0, 0].GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.Font.IsBold = true;
            worksheet.Cells[0, 0].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("MergedCellsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


