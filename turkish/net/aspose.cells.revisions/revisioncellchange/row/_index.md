---
title: "RevisionCellChange.Row"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellChange özelliği. Hücrenin satır indeksini alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellchange/row/
---
## RevisionCellChange.Row property

Hücrenin satır indeksini alır.

```csharp
public int Row { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellChangePropertyRowDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir revizyon oluşturmak için başlangıç verilerini ekle
            worksheet.Cells["B5"].PutValue("Original Value");

            // Hücreyi değiştirerek bir revizyon oluştur
            worksheet.Cells["B5"].PutValue("Modified Value");

            try
            {
                // Revizyon günlüklerine erişin
                RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;
                foreach (RevisionLog log in revisionLogs)
                {
                    foreach (Revision revision in log.Revisions)
                    {
                        if (revision is RevisionCellChange cellChange)
                        {
                            // Row özelliği değerini göster
                            Console.WriteLine("Cell Name: " + cellChange.CellName);
                            Console.WriteLine("Row Index: " + cellChange.Row);
                            Console.WriteLine("Column Index: " + cellChange.Column);
                            Console.WriteLine("Old Value: " + cellChange.OldValue);
                            Console.WriteLine("New Value: " + cellChange.NewValue);

                            // Row özelliğini kullanmayı göster
                            if (cellChange.Row >= 0)
                            {
                                Console.WriteLine("\nThe revision occurred in row " +
                                    (cellChange.Row + 1) + " (1-based index)");
                            }
                        }
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("RevisionCellChangePropertyRowDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [RevisionCellChange](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


