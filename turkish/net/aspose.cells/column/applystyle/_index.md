---
title: "Column.ApplyStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Column yöntemi. Bir bütün sütun için biçimleri uygular"
type: docs
url: /tr/net/aspose.cells/column/applystyle/
---
## Column.ApplyStyle method

Tüm bir sütun için biçimleri uygular.

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
    public class ColumnMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Sütun 2'de çok satırlı metni ayarla
            sheet.Cells[0, 1].Value = "Line1\nLine2";
            sheet.Cells[1, 1].Value = "Text with\nmultiple lines";
            sheet.Cells[2, 1].Value = "Another\nmulti-line\ntext";

            // Metin kaydırma etkinleştirilmiş bir stil oluştur
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // Stili yalnızca sütun 2'nin metin kaydırma özelliğine uygula
            sheet.Cells.Columns[1].ApplyStyle(style, new StyleFlag() { WrapText = true });

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


