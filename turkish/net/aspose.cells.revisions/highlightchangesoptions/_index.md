---
title: "Sınıf HighlightChangesOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.HighlightChangesOptions sınıfı. Paylaşılan Excel dosyalarının revizyonlarını veya değişikliklerini vurgulama seçeneklerini temsil eder."
type: docs
url: /tr/net/aspose.cells.revisions/highlightchangesoptions/
---
## HighlightChangesOptions class

Paylaşılan Excel dosyalarının revizyonlarını veya değişikliklerini vurgulama seçeneklerini temsil eder.

```csharp
public class HighlightChangesOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HighlightChangesOptions](highlightchangesoptions/)(bool, bool) | Paylaşılan Excel dosyalarının revizyonlarını veya değişikliklerini vurgulama seçeneklerini temsil eder. |

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Revisions;
using System;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsDemo
    {
        public static void HighlightChangesExample()
        {
            // Bir Workbook nesnesi oluşturun
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Revizyon günlüklerini al
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Geçmişi korumak için gün sayısını ayarla
            revisionLogs.DaysPreservingHistory = 30;

            // HighlightChangesOptions oluştur
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Değişiklikleri vurgula
            revisionLogs.HighlightChanges(options);

            // Çalışma kitabını vurgulanan değişikliklerle kaydedin
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


