---
title: "RevisionCellComment.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellComment özelliği. Yorum içeren satır indeksini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellcomment/row/
---
## RevisionCellComment.Row property

Yorumu içeren satırın dizinini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellCommentPropertyRowDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // D4 hücresine (satır 3, sütun 3) bir yorum ekle
            int commentRow = 3;
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
                    
                    // Row özelliği değerini göster
                    Console.WriteLine("Comment is located at row: " + commentRevision.Row);
                    
                    // Row özelliğinin kullanımını göster
                    Console.WriteLine("Comment location details:");
                    Console.WriteLine("Row index: " + commentRevision.Row);
                    Console.WriteLine("Column index: " + commentRevision.Column);
                    Console.WriteLine("Cell name: " + commentRevision.CellName);
                    
                    // Row'un yalnızca okunabilir olduğunu, onu değiştirmeye çalışarak göster (derleme hatasına neden olur)
                    // commentRevision.Row = 5; // Bu satır, Row yalnızca okunabilir olduğu için yorum satırı olarak eklenmiştir
                    
                    // CellName'i değiştirerek konumu değiştirmek için alternatif yol
                    Console.WriteLine("\nChanging comment position via CellName...");
                    commentRevision.CellName = "F10"; // Changes to row 9, column 5
                    Console.WriteLine("New Row index: " + commentRevision.Row);
                    Console.WriteLine("New Column index: " + commentRevision.Column);
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionCellCommentPropertyRowDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionCellComment](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


