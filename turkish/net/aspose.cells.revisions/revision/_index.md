---
title: "Class Revision"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Revisions.Revision class. Revizyonu temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revision/
---
## Revision class

Revizyonu temsil eder.

```csharp
public abstract class Revision
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Bu revizyonun numarasını alır. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Revizyonun türünü temsil eder. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Çalışma sayfasını alır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Revizyon oluşturma ihtimali için bazı veriler ekle
                worksheet.Cells["A1"].PutValue("Original Value");

                // Temel bir durum oluşturmak için çalışma kitabını kaydet
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Çalışma kitabını yükle ve bir değişiklik yap
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Herhangi bir revizyon kaydı olup olmadığını kontrol et
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // İlk revizyonu al
                        Revision revision = log.Revisions[0];

                        // Yalnızca okunabilir özellikleri göster
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Değiştirilmiş çalışma kitabını kaydet
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


