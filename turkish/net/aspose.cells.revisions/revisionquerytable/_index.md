---
title: "Sınıf RevisionQueryTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionQueryTable sınıfı. Sorgu tablosu alanı değişikliğinin bir revizyonunu temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Sorgu tablosu alan değişikliğinin bir revizyonunu temsil eder.

```csharp
public class RevisionQueryTable : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Etkilenen sorgu tablosunun konumunu alır. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Kaldırılan belirli sorgu tablosu alanının kimliğini alır. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Sorgu tablosu için bir bağlam oluşturmak amacıyla örnek veri ekleyin
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Not: RevisionQueryTable örnekleri genellikle çalışma kitabı revizyonlarından elde edilir
                // Bu, RevisionQueryTable'ı doğrudan örnekleyemediğimiz için kavramsal bir gösterimdir

                // Gerçek bir senaryoda, revizyonlara şu şekilde erişirsiniz:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Özelliklere eriş
                //     }
                // }

                // Gösterim amacıyla, RevisionQueryTable özellikleriyle nasıl çalışılacağını göstereceğiz
                // eğer bir örnek olsaydı
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


