---
title: "Row.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Satır yöntemi. Bu satırın stilini ayarlar"
type: docs
url: /tr/net/aspose.cells/row/setstyle/
---
## Row.SetStyle method

Bu satırın stilini ayarlar.

```csharp
public void SetStyle(Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | bu satırdaki hücreler için varsayılan stil olarak kullanılacak stil. |

### Açıklamalar

Bu yöntem yalnızca verilen stili bu satır için varsayılan stil olarak ayarlar, aynı satırdaki mevcut hücrelerin stil ayarlarını değiştirmez. Mevcut hücrelerin stil ayarlarını aynı anda belirtilen stile güncellemek için lütfen [`ApplyStyle`](../applystyle/) kullanın.

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir stil oluşturun ve yapılandırın
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Blue;
            style.ForegroundColor = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.DiagonalStripe;

            // İlk satırı alın ve stili uygulayın
            Row row = worksheet.Cells.Rows[0];
            row.SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("RowStyleDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


