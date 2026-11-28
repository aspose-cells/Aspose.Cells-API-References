---
title: "Revision.Worksheet"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Revision özelliği. Çalışma sayfasını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revision/worksheet/
---
## Revision.Worksheet property

Çalışma sayfasını alır.

```csharp
public Worksheet Worksheet { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfası özelliklerini ayarla
            worksheet.Name = "Demo Sheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.DisplayZeros = false;
            worksheet.Zoom = 120;
            
            // Revizyonları göstermek için bazı veri ekleyin
            worksheet.Cells["A1"].PutValue("Original Value");
            
            // Değişiklik takibini etkinleştirmek için çalışma sayfasını koruyun
            worksheet.Protect(ProtectionType.All);
            
            // Revizyon olarak izlenecek bir değişiklik yapın
            worksheet.Cells["A1"].PutValue("Modified Value");
            
            // Revizyonları izlemek için çalışma kitabını kaydedin
            workbook.Save("RevisionDemo.xlsx");
            
            // Revizyonlu çalışma kitabını yükleyin
            Workbook workbookWithRevisions = new Workbook("RevisionDemo.xlsx");
            
            // Revizyon günlüklerine erişin
            foreach (RevisionLog log in workbookWithRevisions.Worksheets.RevisionLogs)
            {
                foreach (Revision revision in log.Revisions)
                {
                    // Revizyondan Worksheet özelliğine erişimi gösterin
                    Console.WriteLine($"Revision Type: {revision.Type}");
                    Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");
                    Console.WriteLine($"Worksheet Index: {revision.Worksheet.Index}");
                    
                    if (revision.Type == RevisionType.ChangeCells)
                    {
                        RevisionCellChange cellChange = (RevisionCellChange)revision;
                        Console.WriteLine($"Cell changed in worksheet '{cellChange.Worksheet.Name}': {cellChange.CellName}");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


