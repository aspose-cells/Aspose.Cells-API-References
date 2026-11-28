---
title: "StyleFlag.Borders"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Tüm kenarlık ayarları uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Tüm kenar ayarları uygulanacak.

```csharp
public bool Borders { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Kenarlık ayarlarıyla bir stil oluşturun
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Bir stil bayrağı oluşturun ve kenarlıkları etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Sadece kenarlıklarla stili A1 hücresine uygulayın
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Çalışma kitabını kaydedin
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


