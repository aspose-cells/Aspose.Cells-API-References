---
title: "RevisionCellMove.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellMove özelliği. Revizyon tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Revizyonun türünü temsil eder.

```csharp
public override RevisionType Type { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Yansıma kullanarak bir RevisionCellMove örneği oluşturun
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Type özelliği değerini göster (yalnızca okunabilir)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Ek bağlamı göster (isteğe bağlı)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("RevisionCellMoveTypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


