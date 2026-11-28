---
title: "StyleFlag.FontName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Yazı tipi adı ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/fontname/
---
## StyleFlag.FontName property

Yazı tipi adı ayarı uygulanacak.

```csharp
public bool FontName { get; set; }
```

### Örnekler

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri oluştur
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(999.99);
            cells["A3"].PutValue("Phone");
            cells["B3"].PutValue(699.99);

            // Farklı yazı tipi adlarıyla stiller oluştur
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.Name = "Arial";
            headerStyle.Font.IsBold = true;
            headerStyle.Font.Size = 14;

            Style priceStyle = workbook.CreateStyle();
            priceStyle.Font.Name = "Courier New";
            priceStyle.Custom = "$#,##0.00";

            // StyleFlag ile başlık stilini uygula
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontName = true;
            headerFlag.FontBold = true;
            headerFlag.FontSize = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            // StyleFlag ile fiyat stilini, Yazı tipi Adına odaklanarak uygula
            Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
            StyleFlag priceFlag = new StyleFlag();
            priceFlag.FontName = true;
            priceFlag.NumberFormat = true;
            priceRange.ApplyStyle(priceStyle, priceFlag);

            // Daha iyi görünürlük için sütunları otomatik sığdır
            worksheet.AutoFitColumns();

            // Çalışma kitabını kaydedin
            workbook.Save("FontNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


