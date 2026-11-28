---
title: "Enum CommentTitleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Rendering.CommentTitleType enum. Yorumun sayfanın sonunda gösterilecek şekilde ayarlandığında, renderleme sırasında yorum başlığı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.rendering/commenttitletype/
---
## CommentTitleType enumeration

Yorumun sayfa sonunda gösterilecek şekilde ayarlandığında, render sırasında yorum başlığı türünü temsil eder.

```csharp
public enum CommentTitleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Cell | `0` | Yorum başlığı hücresini temsil eder. |
| Comment | `1` | Yorum başlığı yorumunu temsil eder. |
| Note | `2` | Yorum başlığı notunu temsil eder. |
| Reply | `3` | Yorum başlığı yanıtını temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassCommentTitleTypeDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Özel küreselleşme ayarları oluşturun
                SettableGlobalizationSettings globalizationSettings = new SettableGlobalizationSettings();

                // Tüm CommentTitleType enum değerlerini gösterin
                Console.WriteLine("Available CommentTitleType values:");
                Console.WriteLine($"Cell: {(int)CommentTitleType.Cell}");
                Console.WriteLine($"Comment: {(int)CommentTitleType.Comment}");
                Console.WriteLine($"Note: {(int)CommentTitleType.Note}");
                Console.WriteLine($"Reply: {(int)CommentTitleType.Reply}");

                // Her yorum türü için özel başlıklar ayarlayın
                globalizationSettings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                globalizationSettings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Küreselleştirme ayarlarını çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = globalizationSettings;

                // İşlevselliği göstermek için bir yorum ekleyin
                int commentIndex = worksheet.Comments.Add("A1");
                Comment comment = worksheet.Comments[commentIndex];
                comment.Note = "This is a test comment";
                comment.Author = "Test Author";

                // Çalışma kitabını kaydedin
                workbook.Save("CommentTitleTypeDemo.xlsx");

                Console.WriteLine("CommentTitleType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in CommentTitleType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


