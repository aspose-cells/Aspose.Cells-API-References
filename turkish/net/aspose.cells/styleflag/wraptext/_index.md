---
title: "StyleFlag.WrapText"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Metni kaydırma ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

Metni kaydırma ayarı uygulanacak.

```csharp
public bool WrapText { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metin kaydırma etkinleştirilmiş bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Bir stil bayrağı oluşturun ve WrapText bayrağını etkinleştirin
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // Stili, belirtilen bayraklarla A1 hücresine uygula
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // Kaydırılmış metni görmek için satır yüksekliğini otomatik ayarla
            worksheet.AutoFitRow(0);

            // Çalışma kitabını kaydedin
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


