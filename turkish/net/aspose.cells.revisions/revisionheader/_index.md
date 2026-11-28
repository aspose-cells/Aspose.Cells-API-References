---
title: "RevisionHeader sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionHeader sınıfı. Bu çalışma kitabı için gerçekleşen belirli değişikliklerin bir listesini temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Bu çalışma kitabı için gerçekleşen belirli değişikliklerin bir listesini temsil eder.

```csharp
public class RevisionHeader
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Bu revizyon seti kaydedildiğinde tarih ve saati alır ve ayarlar |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Revizyonu yapan kullanıcının adını alır ve ayarlar |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // RevisionHeader sınıfının bir örneğini oluşturun
                RevisionHeader revisionHeader = new RevisionHeader();

                // Temel özellikleri ayarlayın
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Temel işlevselliği gösterin
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


