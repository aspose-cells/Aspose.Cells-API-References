---
title: "Font.CapsType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Metin büyük harf tipini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/capstype/
---
## Font.CapsType property

Metin büyük harf tipini alır ve ayarlar.

```csharp
[Obsolete("Use TextOptions.CapsType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public TextCapsType CapsType { get; set; }
```

### Açıklamalar

Yalnızca Şekil veya Grafik yazı tipleri için. NOT: Bu üye artık kullanılmamaktadır. Bunun yerine lütfen [`CapsType`](../../../aspose.cells.drawing.texts/textoptions/capstype/) özelliğini kullanın. Bu özellik Ocak 2026'dan itibaren 12 ay içinde kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyCapsTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("sample text");

            Style style = cell.GetStyle();
            style.Font.CapsType = TextCapsType.All;
            cell.SetStyle(style);

            workbook.Save("FontCapsTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


