---
title: "RevisionCellMove.DestinationArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RevisionCellMove özelliği. Hedef alanı alır"
type: docs
url: /tr/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Hedef alanı alır.

```csharp
public CellArea DestinationArea { get; }
```

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // Geçerli bir ortam sağlamak için bir çalışma kitabı oluşturun (demo için isteğe bağlı)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Yansıma yoluyla RevisionCellMove'i örnekleyin (parametresiz ctor)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // DestinationArea özelliğini okuyun ve görüntüleyin (yalnızca okunur)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Ek bağlam (isteğe bağlı)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Çalışma kitabını kaydedin (isteğe bağlı)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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


