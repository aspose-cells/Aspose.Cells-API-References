---
title: "RevisionLog.MetadataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionLog özelliği. Bu çalışma kitabında gerçekleşen belirli değişikliklerin bir listesi hakkında meta verileri içeren tabloyu alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisionlog/metadatatable/
---
## RevisionLog.MetadataTable property

Bu çalışma kitabında gerçekleşen belirli değişikliklerin bir listesinin meta verilerini içeren tabloyu alır.

```csharp
public RevisionHeader MetadataTable { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionLogPropertyMetadataTableDemo
    {
        public static void Run()
        {
            // Örnek verilerle yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Revizyon geçmişi oluşturmak için bazı değişiklikler yapın
            worksheet.Cells["A1"].PutValue("Original Value");
            workbook.Save("RevisionDemo.xlsx", SaveFormat.Xlsx);
            
            // Hücreyi değiştirerek bir revizyon oluştur
            worksheet.Cells["A1"].PutValue("Modified Value");
            workbook.Save("RevisionDemo_modified.xlsx", SaveFormat.Xlsx);

            // Revizyon günlüklerine erişmek için değiştirilmiş çalışma kitabını yeniden aç
            workbook = new Workbook("RevisionDemo_modified.xlsx");
            
            // Revizyon günlüklerine erişin
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
            
            if (revisionLogs.Count > 0)
            {
                RevisionLog revisionLog = revisionLogs[0];
                RevisionHeader metadata = revisionLog.MetadataTable;
                
                Console.WriteLine("Revision Metadata:");
                Console.WriteLine("Saved Time: " + metadata.SavedTime);
                Console.WriteLine("Modified By: " + metadata.UserName);
                Console.WriteLine("Number of Revisions: " + revisionLog.Revisions.Count);
            }
            else
            {
                Console.WriteLine("No revision history found");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [RevisionHeader](../../revisionheader/)
* class [RevisionLog](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


