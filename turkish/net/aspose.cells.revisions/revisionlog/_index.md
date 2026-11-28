---
title: "Sınıf RevisionLog"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.RevisionLog sınıfı. Revizyon günlüğünü temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/revisionlog/
---
## RevisionLog class

Revizyon günlüğünü temsil eder.

```csharp
public class RevisionLog
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [MetadataTable](../../aspose.cells.revisions/revisionlog/metadatatable/) { get; } | Bu çalışma kitabında gerçekleşen belirli değişikliklerin bir listesinin meta verilerini içeren tabloyu alır. |
| [Revisions](../../aspose.cells.revisions/revisionlog/revisions/) { get; } | Bu günlükteki tüm revizyonları alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogDemo
    {
        public static void RevisionLogExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Çalışma kitabının revizyon günlüklerine erişin
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Herhangi bir revizyon kaydı olup olmadığını kontrol et
            if (revisionLogs.Count > 0)
            {
                // İlk revizyon günlüğüne erişin
                RevisionLog revisionLog = revisionLogs[0];

                // Revizyon günlüğünün meta veri tablosuna erişin
                RevisionHeader metadataTable = revisionLog.MetadataTable;

                // Revizyon günlüğündeki revizyonlara erişin
                RevisionCollection revisions = revisionLog.Revisions;

                // Revizyonlar hakkında bazı bilgileri gösterin
                Console.WriteLine("Number of revisions: " + revisions.Count);
                Console.WriteLine("Metadata Table: " + metadataTable.ToString());
            }
            else
            {
                Console.WriteLine("No revision logs found.");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("RevisionLogExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


