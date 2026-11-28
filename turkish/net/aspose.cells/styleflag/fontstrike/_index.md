---
title: "StyleFlag.FontStrike"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Yazı tipi üzeri çizgi ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

Yazı tipi üstü çizili ayarı uygulanacak.

```csharp
public bool FontStrike { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Bir stil nesnesi oluşturun ve FontStrike'i true olarak ayarlayın
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // Bir stil bayrağı oluşturun ve FontStrike bayrağını etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // Stil bayrağıyla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Mevcut FontStrike durumunu göster
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // Üstü çizili olmayan metni göstermek için başka bir hücre oluşturun
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // Etkileri görmek için çalışma kitabını kaydedin
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


