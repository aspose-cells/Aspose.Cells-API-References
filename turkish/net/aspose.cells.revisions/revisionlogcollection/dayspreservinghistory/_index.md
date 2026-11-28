---
title: "RevisionLogCollection.DaysPreservingHistory"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionLogCollection özelliği. Bu çalışma kitabı için elektronik tablo uygulamasının değişiklik geçmişini tutacağı gün sayısını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.revisions/revisionlogcollection/dayspreservinghistory/
---
## RevisionLogCollection.DaysPreservingHistory property

Bu çalışma kitabı için elektronik tablo uygulamasının değişiklik geçmişini tutacağı gün sayısını alır ve ayarlar.

```csharp
public int DaysPreservingHistory { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RevisionLogCollectionPropertyDaysPreservingHistoryDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Settings.Shared = true;
            workbook.Worksheets[0].Cells["A1"].PutValue("Test Value");
            
            // DaysPreservingHistory özelliğini ayarla
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 40;
            
            string outputPath = "output_DaysPreservingHistory.xlsx";
            workbook.Save(outputPath);
            
            // Özelliği doğrulamak için yeniden yükle
            Workbook loadedWorkbook = new Workbook(outputPath);
            Console.WriteLine("DaysPreservingHistory: " + 
                loadedWorkbook.Worksheets.RevisionLogs.DaysPreservingHistory);
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


