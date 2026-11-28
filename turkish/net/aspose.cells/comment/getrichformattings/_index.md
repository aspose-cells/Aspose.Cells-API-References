---
title: "Comment.GetRichFormattings"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment yöntemi. Yorum metni içinde bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür."
type: docs
url: /tr/net/aspose.cells/comment/getrichformattings/
---
## Comment.GetRichFormattings method

Yorum metni içindeki bir karakter aralığını temsil eden tüm Characters nesnelerini döndürür.

```csharp
public FontSetting[] GetRichFormattings()
```

### Dönüş Değeri

Tüm Characters nesneleri

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodGetRichFormattingsDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.HtmlNote = "<b>Bold</b>, <i>Italic</i>, <u>Underline</u>";

            // Zengin metin biçimlendirmelerini al
            FontSetting[] formattings = comment.GetRichFormattings();

            // Biçimlendirme bilgilerini göster
            Console.WriteLine("Rich Text Formattings:");
            foreach (FontSetting setting in formattings)
            {
                Console.WriteLine($"StartIndex: {setting.StartIndex}, Length: {setting.Length}");
                Console.WriteLine($"Bold: {setting.Font.IsBold}, Italic: {setting.Font.IsItalic}, Underline: {setting.Font.Underline}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


