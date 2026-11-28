---
title: "Sınıf RevisionFormat"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionFormat sınıfı. Biçimlendirme değişikliğiyle ilgili bilgi içeren bir revizyon kaydını temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionformat/
---
## RevisionFormat class

Biçimlendirme değişikliği hakkında bilgi içeren bir revizyon kaydını temsil eder.

```csharp
public class RevisionFormat : Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Areas](../../aspose.cells.revisions/revisionformat/areas/) { get; } | Bu biçimlendirmenin uygulandığı aralık. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır.(Inherited from [`Revision`](../revision/).) |
| [Style](../../aspose.cells.revisions/revisionformat/style/) { get; } | Uygulanan stili alır. |
| override [Type](../../aspose.cells.revisions/revisionformat/type/) { get; } | Revizyon tipini alır. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. ([`Revision`](../revision/) üzerinden devralınmıştır.) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionFormatDemo
    {
        public static void Run()
        {
            // Revizyon izlemeyi etkinleştirmek için paylaşımlı modda yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Bir revizyon oluşturmak için bazı veriler ekleyin ve biçimlendirme uygulayın
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("Sample Data");

                // Biçim revizyonu oluşturmak için bir stil uygulayın
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                cell.SetStyle(style);

                // Revizyon günlüklerine erişin
                foreach (RevisionLog revisionLog in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision revision in revisionLog.Revisions)
                    {
                        if (revision is RevisionFormat revisionFormat)
                        {
                            // Revizyon özelliklerini göster
                            Console.WriteLine("Revision Type: " + revisionFormat.Type);
                            Console.WriteLine("Number of affected areas: " + revisionFormat.Areas.Length);

                            // Stil bilgilerini göster
                            Style revisionStyle = revisionFormat.Style;
                            Console.WriteLine("Font Name: " + revisionStyle.Font.Name);
                            Console.WriteLine("Font Size: " + revisionStyle.Font.Size);
                            Console.WriteLine("Is Bold: " + revisionStyle.Font.IsBold);
                        }
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionFormatDemo.xlsx");
                Console.WriteLine("RevisionFormat demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionFormat: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


