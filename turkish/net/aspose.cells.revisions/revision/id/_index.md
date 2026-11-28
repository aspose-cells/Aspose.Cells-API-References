---
title: "Revision.Id"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Revision özelliği. Bu revizyonun numarasını alır"
type: docs
url: /tr/net/aspose.cells.revisions/revision/id/
---
## Revision.Id property

Bu revizyonun numarasını alır.

```csharp
public int Id { get; }
```

### Açıklamalar

Sıfır, bu revizyonun kimlik içermediği anlamına gelir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionPropertyIdDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir değişiklik yaparak potansiyel olarak bir revizyon oluşturun
            worksheet.Cells["A1"].Value = "Sample Data";
            
            try
            {
                // Revizyon günlükleri koleksiyonunu al
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                
                if (revisionLogs != null && revisionLogs.Count > 0)
                {
                    // İlk günlükten revizyonları al
                    RevisionCollection revisions = revisionLogs[0].Revisions;
                    
                    if (revisions != null && revisions.Count > 0)
                    {
                        // İlk revizyona eriş
                        Revision revision = revisions[0];
                        
                        // Id özelliğini göster (yalnızca okunabilir)
                        Console.WriteLine("Revision Id: " + revision.Id);
                        
                        // Çalışma kitabını kaydedin
                        workbook.Save("RevisionIdDemo.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs were created");
                }
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

* class [Revision](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


