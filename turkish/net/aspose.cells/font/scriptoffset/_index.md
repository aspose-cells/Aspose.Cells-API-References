---
title: "Font.ScriptOffset"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Font özelliği. Yüzde biriminde script offsetini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/font/scriptoffset/
---
## Font.ScriptOffset property

Komut ofsetini yüzde biriminde alır ve ayarlar.

```csharp
public double ScriptOffset { get; set; }
```

### Açıklamalar

Yalnızca şekiller ve grafikler için.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyScriptOffsetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine eriş ve değerini ayarla
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("ScriptOffset Demo");

            // Hücrenin stilini ve fontunu al
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Alt/üst simge etkisini göstermek için ScriptOffset'i ayarla
            font.ScriptOffset = 10; // Positive for superscript, negative for subscript
            font.IsSuperscript = true; // Enable superscript

            // Değiştirilmiş stili hücreye geri uygula
            cell.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("FontScriptOffsetDemo.xlsx");

            // ScriptOffset değerini doğrula
            Console.WriteLine("ScriptOffset value: " + font.ScriptOffset);
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


