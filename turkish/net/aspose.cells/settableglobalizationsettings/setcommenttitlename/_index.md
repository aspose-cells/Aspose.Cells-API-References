---
title: "SettableGlobalizationSettings.SetCommentTitleName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SettableGlobalizationSettings yöntemi. Yorum başlığı türüne göre yerel bağımlı yorum başlığı adını alır"
type: docs
url: /tr/net/aspose.cells/settableglobalizationsettings/setcommenttitlename/
---
## SettableGlobalizationSettings.SetCommentTitleName method

Yorum başlığı türüne göre yerel ayara bağlı yorum başlığı adını alır.

```csharp
public void SetCommentTitleName(CommentTitleType type, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | CommentTitleType | yorum başlığı tipi |
| name | String | yerel ayara bağlı yorum başlığı adı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class SettableGlobalizationSettingsMethodSetCommentTitleNameWithCommentTitleTypeStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine bir yorum ekle
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            comment.IsVisible = true;

            // Küreselleştirme ayarları oluştur
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();

            try
            {
                // Farklı türler için özel yorum başlığı adlarını ayarla
                settings.SetCommentTitleName(CommentTitleType.Cell, "Custom Cell Title");
                settings.SetCommentTitleName(CommentTitleType.Comment, "Custom Comment Title");
                settings.SetCommentTitleName(CommentTitleType.Note, "Custom Note Title");
                settings.SetCommentTitleName(CommentTitleType.Reply, "Custom Reply Title");

                // Küreselleştirme ayarlarını çalışma kitabına uygula
                workbook.Settings.GlobalizationSettings = settings;

                Console.WriteLine("SetCommentTitleName method executed successfully with parameters (CommentTitleType, String)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetCommentTitleName method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("MethodSetCommentTitleNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [CommentTitleType](../../../aspose.cells.rendering/commenttitletype/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


