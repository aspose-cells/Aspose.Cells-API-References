---
title: "StyleFlag.FontScript"
second_title: "Aspose.Cells için .NET API Referansı"
description: "StyleFlag özelliği. Yazı tipi betik ayarı uygulanacak"
type: docs
url: /tr/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

Yazı tipi betik ayarı uygulanacak.

```csharp
public bool FontScript { get; set; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bazı metinler ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // Bir stil nesnesi oluşturun ve yazı tipi betiğini alt simgeye ayarlayın
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // Bir stil bayrağı oluşturun ve FontScript bayrağını etkinleştirin
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // Stil bayrağıyla stili hücreye uygulayın
            cell.SetStyle(style, styleFlag);

            // Mevcut yazı tipi betik durumunu göster
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Yazı tipi betiğini üst simgeye değiştir
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // Güncellenmiş yazı tipi betik durumunu göster
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // Çalışma kitabını kaydedin
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


