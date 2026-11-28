---
title: "Range.ApplyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Range yöntemi. Tüm bir aralık için biçimleri uygular"
type: docs
url: /tr/net/aspose.cells/range/applystyle/
---
## Range.ApplyStyle method

Tüm bir aralık için biçimlendirmeleri uygular

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Açıklamalar

Bu aralıktaki her hücre bir [`Style`](../../style/) nesnesi içerir. Bu nedenle bellek tüketen bir yöntemdir. Lütfen dikkatli kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Style style = workbook.CreateStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;
            style.IsTextWrapped = true;

            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 0].PutValue("Sample text for style demonstration");

            Aspose.Cells.Range range = cells.CreateRange(0, 0, 1, 3);

            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            styleFlag.VerticalAlignment = true;
            styleFlag.WrapText = true;

            range.ApplyStyle(style, styleFlag);

            workbook.Save("ApplyStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


