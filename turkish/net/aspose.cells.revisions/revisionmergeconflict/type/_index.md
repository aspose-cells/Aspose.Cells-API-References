---
title: "RevisionMergeConflict.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionMergeConflict özelliği. Revizyonun türünü alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionmergeconflict/type/
---
## RevisionMergeConflict.Type property

Revizyon tipini alır.

```csharp
public override RevisionType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionMergeConflictPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Değişiklik izlemeyi etkinleştir
            workbook.StartAccessCache(AccessCacheOptions.All);

            // Bir birleştirme çakışması senaryosu oluşturmak için değişiklikler yapın
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("TempMergeConflict.xlsx");

            // Dosyayı açıp çakışan değişiklikler yaparak bir birleştirme çakışmasını simüle edin
            Workbook otherUserWorkbook = new Workbook("TempMergeConflict.xlsx");
            otherUserWorkbook.Worksheets[0].Cells["A1"].PutValue("Conflicting Change");
            otherUserWorkbook.Save("TempMergeConflict_OtherUser.xlsx");

            // Çakışan değişiklikleri birleştirin
            workbook.Combine(otherUserWorkbook);

            // Revizyonların olup olmadığını kontrol edin
            if (workbook.HasRevisions)
            {
                // Birleştirme çakışması revizyonunu bulun
                RevisionMergeConflict mergeConflictRevision = null;
                // Not: Gerçek uygulamada, revizyonlara erişmek için başka bir yola ihtiyacınız olur
                // çünkü Revisions özelliği sağlanan API tanımında mevcut değil

                if (mergeConflictRevision != null)
                {
                    // Birleştirme çakışması revizyonunun Type özelliğini gösterin
                    Console.WriteLine("Merge Conflict Revision Type: " + mergeConflictRevision.Type);

                    // Bu bilginin nasıl kullanılabileceğini gösterin
                    if (mergeConflictRevision.Type == RevisionType.MergeConflict)
                    {
                        Console.WriteLine("This revision represents a merge conflict.");
                        Console.WriteLine("Worksheet affected: " + mergeConflictRevision.Worksheet.Name);
                    }
                }
            }

            // Revizyonlarla birlikte çalışma kitabını kaydet
            workbook.Save("RevisionMergeConflictTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RevisionType](../../revisiontype/)
* class [RevisionMergeConflict](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


