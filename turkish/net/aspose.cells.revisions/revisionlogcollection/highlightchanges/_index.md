---
title: "RevisionLogCollection.HighlightChanges"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionLogCollection yöntemi. Paylaşılan çalışma kitabının değişikliklerini vurgular"
type: docs
url: /tr/net/aspose.cells.revisions/revisionlogcollection/highlightchanges/
---
## RevisionLogCollection.HighlightChanges method

Paylaşılan çalışma kitabının değişikliklerini vurgular.

```csharp
public void HighlightChanges(HighlightChangesOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| seçenekler | HighlightChangesOptions | Hangi değişikliklerin izleneceğini filtrelemek için seçenekleri ayarla. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionMethodHighlightChangesWithHighlightChangesOptionsDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bazı örnek veri ve revizyonlar ekle
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Seçeneklerle değişiklikleri vurgulayın
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            workbook.Worksheets.RevisionLogs.HighlightChanges(options);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HighlightChangesOptions](../../highlightchangesoptions/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


