---
title: "Row.ApplyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Row yöntemi. Bir bütün satır için biçimleri uygular"
type: docs
url: /tr/net/aspose.cells/row/applystyle/
---
## Row.ApplyStyle method

Tüm satır için biçimleri uygular.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Uygulanacak stil nesnesi. |
| bayrak | StyleFlag | Uygulanan biçimlendirme özelliklerini gösteren bayraklar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // İlk hücrede HTML içeriği ayarla
            sheet.Cells[0, 0].HtmlString = @"<font style=""color: #49c131; font-weight: bold;"">Styled </font><font>text</font>";

            // İlk satırı ve stilini al
            Row row = sheet.Cells.Rows[0];
            Style style = row.GetStyle();
            
            // Stil özelliklerini değiştir
            style.IsTextWrapped = true;
            style.HorizontalAlignment = TextAlignmentType.Center;

            // Belirli bayraklarla stili uygula (yalnızca metni kaydırma uygulanacak)
            row.ApplyStyle(style, new StyleFlag { WrapText = true });

            // Demonstrasyon için otomatik sığdırma
            sheet.AutoFitRows();
            sheet.AutoFitColumns();

            // Çalışma kitabını kaydedin
            workbook.Save("RowApplyStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


