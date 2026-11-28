---
title: "RevisionLogCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionLogCollection özelliği. RevisionLog'u indeksle alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

İndeksle [`RevisionLog`](../../revisionlog/) alır.

```csharp
public RevisionLog this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Dönüş Değeri

[`RevisionLog`](../../revisionlog/) nesnesini döndürür.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Revizyonları desteklemek için paylaşılan çalışma kitabını etkinleştir
            workbook.Settings.Shared = true;

            // Revizyon günlükleri koleksiyonuna erişin
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Herhangi bir revizyon kaydı olup olmadığını kontrol et
                if (revisionLogs.Count > 0)
                {
                    // Item özelliğini kullanarak ilk revizyon günlüğüne eriş
                    RevisionLog firstLog = revisionLogs[0];

                    // Revizyon günlüğü hakkında temel bilgileri göster
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


