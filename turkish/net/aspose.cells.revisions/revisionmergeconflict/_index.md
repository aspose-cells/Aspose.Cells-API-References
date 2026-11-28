---
title: "Sınıf RevisionMergeConflict"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionMergeConflict sınıfı. Bir birleştirme çakışması olduğunu gösteren bir revizyon kaydını temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/revisionmergeconflict/
---
## RevisionMergeConflict class

Bir birleştirme çakışması olduğunu gösteren bir revizyon kaydını temsil eder.

```csharp
public class RevisionMergeConflict : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionmergeconflict/type/) { get; } | Revizyon tipini alır. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionsClassRevisionMergeConflictDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Revizyon geçmişi oluşturmak için bazı değişiklikler yapın
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue("Another Value");

            // Revizyonlar oluşturmak için çalışma kitabını kaydedin
            workbook.Save("RevisionMergeConflictDemo_Before.xlsx");

            // Bir birleştirme çakışması senaryosu oluşturun
            worksheet.Cells["A1"].PutValue("Conflicting Change 1");
            worksheet.Cells["A1"].PutValue("Conflicting Change 2");

            // Revizyon geçmişini alın (RevisionLogCollection üzerinden doğrudan yineleyin)
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // RevisionMergeConflict'i bulun ve gösterin
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionMergeConflict mergeConflict)
                    {
                        // Revizyon tipine erişimi gösterin
                        RevisionType revisionType = mergeConflict.Type;
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionMergeConflictDemo_After.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


