---
title: "RevisionCellComment.Column"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellComment özelliği. Yorum içeren sütunun indeksini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellcomment/column/
---
## RevisionCellComment.Column property

Yorumu içeren sütunun dizinini alır.

```csharp
public int Column { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // D3 hücresine bir yorum ekleyin
            int commentRow = 2;
            int commentCol = 3;
            Comment comment = worksheet.Comments[commentRow, commentCol];
            comment.Note = "Sample comment for revision tracking";

            // Bir revizyon oluşturmak için yorumu değiştir
            comment.Note = "Updated comment text";

            // Revizyonlara eriş
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;
                    
                    // Column özelliğinin değerini göster
                    Console.WriteLine("Comment revision column index: " + commentRevision.Column);
                    
                    // Column özelliğinin kullanımını göster
                    Console.WriteLine("Comment was modified in column: " + (char)('A' + commentRevision.Column));
                    
                    // İlgili özellikleri göster
                    Console.WriteLine("Associated row: " + commentRevision.Row);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Not: Column yalnızca okunabilir, bu yüzden doğrudan değiştiremeyiz
                    // CellName'i değiştirerek dolaylı olarak değiştirebiliriz
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "E5"; // This will update both Row and Column properties
                    Console.WriteLine("After CellName change - New column: " + commentRevision.Column);
                    
                    // Orijinal değeri geri yükle
                    commentRevision.CellName = originalCellName;
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionCellCommentPropertyColumnDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


