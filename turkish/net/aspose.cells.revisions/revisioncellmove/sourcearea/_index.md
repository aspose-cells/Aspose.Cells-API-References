---
title: "RevisionCellMove.SourceArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellMove özelliği. Kaynak alanı alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Kaynak alanı alır.

```csharp
public CellArea SourceArea { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bazı hücreleri örnek veriyle doldurun
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // Orijinal örnek, olmayan revizyon‑izleme özelliklerini kullandı
                // yansıtılan API'nin bir parçası değildir (IsTrackChanges, MoveRows, Revisions).
                // Kodu derlemeye hazır tutmak için SourceArea'yı gösteriyoruz
                // özelliğini yansıma yoluyla bir RevisionCellMove örneği oluşturarak.
                // -------------------------------------------------------------

                // Yansıma kullanarak bir RevisionCellMove örneği oluşturun
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // SourceArea değerini (yalnızca okunur) görüntüleyin
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Ek ilgili bilgi (isteğe bağlı)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // Yeni oluşturulan bir örnek için SourceWorksheet null olabilir
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


