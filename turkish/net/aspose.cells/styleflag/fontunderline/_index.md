---
title: "StyleFlag.FontUnderline"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Yazı tipi alt çizgi ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

Yazı tipi altı çizili ayarı uygulanacak.

```csharp
public bool FontUnderline { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // Bir stil nesnesi oluştur ve yazı tipi alt çizgisini ayarla
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // Bir stil bayrağı oluşturun ve yazı tipi alt çizgi bayrağını etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // Stil bayrağıyla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Mevcut alt çizgi durumunu gösterin
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Alt çizgi tipini çift olarak değiştirin
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // Çalışma kitabını kaydedin
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


