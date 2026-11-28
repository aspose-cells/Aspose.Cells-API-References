---
title: "Comment.Characters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment yöntemi. Yorum metni içinde bir karakter aralığını temsil eden bir Characters nesnesi döndürür"
type: docs
url: /tr/net/aspose.cells/comment/characters/
---
## Comment.Characters method

Yorum metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Karakterin başlangıç indeksidir. |
| uzunluk | Int32 | Karakter sayısı. |

### Dönüş Değeri

Karakterler nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";
            
            // İlk 4 karakter için yazı tipi ayarını al
            FontSetting fontSetting = comment1.Characters(0, 4);
            
            // Yazı tipi ayarlarını değiştir
            fontSetting.Font.Color = System.Drawing.Color.Red;
            fontSetting.Font.IsBold = true;
            
            // Çalışma kitabını kaydedin
            workbook.Save("CommentFontSettingDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [FontSetting](../../fontsetting/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


