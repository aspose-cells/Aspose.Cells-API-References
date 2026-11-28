---
title: "PaneCollection.AcitvePaneType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaneCollection özelliği. Etkin bölmeyi alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Etkin bölmeyi alır ve ayarlar.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Açıklamalar

NOT: Bu özellik artık kullanımdan kaldırılmıştır. Bunun yerine lütfen [`ActivePaneType`](../activepanetype/) özelliğini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bölme bölme işlemini göstermek için örnek veri ekleyin
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Çalışma sayfasını bölmelere ayırın
            worksheet.Split();

            // Bölme koleksiyonunu alın
            PaneCollection panes = worksheet.GetPanes();

            // Mevcut etkin bölmeyi göster
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Etkin bölmeyi BottomRight olarak ayarlayın
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Alt/sağ bölmeler için ilk görünen satır/sütunu ayarlayın
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Çalışma kitabını kaydedin
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


