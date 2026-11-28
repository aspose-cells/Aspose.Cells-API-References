---
title: "Comment.FormatCharacters"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Comment yöntemi. Bazı karakterleri yazı tipi ayarıyla biçimlendir"
type: docs
url: /tr/net/aspose.cells/comment/formatcharacters/
---
## Comment.FormatCharacters method

Bazı karakterleri yazı tipi ayarıyla biçimlendir.

```csharp
public void FormatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startIndex | Int32 | Başlangıç indeksi. |
| uzunluk | Int32 | Uzunluk. |
| yazı tipi | Yazı Tipi | Yazı tipi ayarı. |
| bayrak | StyleFlag | Yazı tipi ayarının bayrağı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CommentMethodFormatCharactersWithInt32Int32FontStyleFlagDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentRow = 0;
            int commentColumn = 0;
            Comment comment = worksheet.Comments[commentRow, commentColumn];
            comment.Note = "This is a sample comment with formatted text.";

            // Biçimlendirme için bir yazı tipi oluştur - çalışma kitabının stilinden alınması gerekir
            Aspose.Cells.Font font = workbook.CreateStyle().Font;
            font.IsBold = true;
            font.Color = Color.Red;
            font.Size = 14;
            font.Underline = FontUnderlineType.Single;

            // Uygulanacak yazı tipi özelliklerini belirtmek için stil bayrağı oluştur
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontBold = true;
            styleFlag.FontColor = true;
            styleFlag.FontSize = true;
            styleFlag.FontUnderline = true;

            try
            {
                // 5. indeksten itibaren, 10 uzunluğunda karakterleri biçimlendir
                comment.FormatCharacters(5, 10, font, styleFlag);

                Console.WriteLine("FormatCharacters method executed successfully on the comment.");
                
                // Etkiyi görmek için yorumu görünür yap
                comment.IsVisible = true;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing FormatCharacters method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("CommentFormatCharactersDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Font](../../font/)
* class [StyleFlag](../../styleflag/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


