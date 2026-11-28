---
title: "Font.IsNormalizeHeights"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Metin akışına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/font/isnormalizeheights/
---
## Font.IsNormalizeHeights property

Metin çalıştırmasına uygulanacak yükseklik normalizasyonunun olup olmadığını gösterir.

```csharp
[Obsolete("Use TextOptions.IsNormalizeHeights property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsNormalizeHeights { get; set; }
```

### Açıklamalar

Yalnızca Şekil veya Grafik yazı tipleri için. NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen [`IsNormalizeHeights`](../../../aspose.cells.drawing.texts/textoptions/isnormalizeheights/) özelliğini kullanın. Bu özellik Ocak 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsNormalizeHeightsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Style style = workbook.CreateStyle();
            Font font = style.Font;

            // IsNormalizeHeights özelliğini ayarla
            font.IsNormalizeHeights = true;
            Console.WriteLine("Font IsNormalizeHeights: " + font.IsNormalizeHeights);

            // Stili bir hücreye uygula
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Test Text");

            // Özelliği doğrula
            Font cellFont = cell.GetStyle().Font;
            Console.WriteLine("Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);

            // Özelliği değiştir
            cellFont.IsNormalizeHeights = false;
            Console.WriteLine("Modified Cell Font IsNormalizeHeights: " + cellFont.IsNormalizeHeights);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


