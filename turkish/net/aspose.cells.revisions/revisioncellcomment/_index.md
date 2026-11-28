---
title: "Sınıf RevisionCellComment"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionCellComment sınıfı. Bir hücre yorum değişikliğinin revizyon kaydını temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellcomment/
---
## RevisionCellComment class

Hücre yorumu değişikliği için bir revizyon kaydını temsil eder.

```csharp
public class RevisionCellComment : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActionType](../../aspose.cells.revisions/revisioncellcomment/actiontype/) { get; } | Revizyonun eylem türünü alır. |
| [CellName](../../aspose.cells.revisions/revisioncellcomment/cellname/) { get; set; } | Hücrenin adını alır. |
| [Column](../../aspose.cells.revisions/revisioncellcomment/column/) { get; } | Yorumu içeren sütunun dizinini alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [IsOldComment](../../aspose.cells.revisions/revisioncellcomment/isoldcomment/) { get; } | Eski bir yorum olup olmadığını gösterir. |
| [NewLength](../../aspose.cells.revisions/revisioncellcomment/newlength/) { get; } | Bu revizyon yapılmadan önce yorumun uzunluğunu alır. |
| [OldLength](../../aspose.cells.revisions/revisioncellcomment/oldlength/) { get; } | Bu revizyonda eklenen yorum metninin uzunluğunu alır. |
| [Row](../../aspose.cells.revisions/revisioncellcomment/row/) { get; } | Yorumu içeren satırın dizinini alır. |
| override [Type](../../aspose.cells.revisions/revisioncellcomment/type/) { get; } | Revizyon tipini alır. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellCommentDemo
    {
        public static void Run()
        {
            // Revizyon takibi ile yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine ilk yorumu ekle
            Comment comment = worksheet.Comments[0, 0];
            comment.Note = "Initial comment text";

            // Bir revizyon oluşturmak için yorumu değiştir
            comment.Note = "Updated comment with more text";

            // Revizyon günlüğüne eriş
            RevisionCollection revisions = workbook.Worksheets.RevisionLogs[0].Revisions;
            foreach (Revision revision in revisions)
            {
                if (revision is RevisionCellComment)
                {
                    RevisionCellComment commentRevision = (RevisionCellComment)revision;

                    // Revizyon özelliklerini göster
                    Console.WriteLine("Revision Type: " + commentRevision.Type);
                    Console.WriteLine("Action Type: " + commentRevision.ActionType);
                    Console.WriteLine("Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("Row: " + commentRevision.Row);
                    Console.WriteLine("Column: " + commentRevision.Column);

                    // Yorum uzunluğu değişikliklerini göster
                    Console.WriteLine("Old Length: " + commentRevision.OldLength);
                    Console.WriteLine("New Length: " + commentRevision.NewLength);
                    Console.WriteLine("Is Old Comment: " + commentRevision.IsOldComment);

                    // Özellik değişikliğini göstermek için hücre adını değiştir
                    string originalCellName = commentRevision.CellName;
                    commentRevision.CellName = "B2";
                    Console.WriteLine("Modified Cell Location: " + commentRevision.CellName);
                    Console.WriteLine("New Row: " + commentRevision.Row);
                    Console.WriteLine("New Column: " + commentRevision.Column);

                    // Orijinal hücre adını geri yükle
                    commentRevision.CellName = originalCellName;
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionsClassRevisionCellCommentDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


