---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaneCollection özelliği. Alt bölmenin ilk görünen satırını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Alt bölmenin ilk görünen satırını alır ve ayarlar.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kaydırılabilir bir bölme oluşturmak için örnek veri ekleyin
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Satır 10'da bölmeleri dondurun (bu, üst ve alt bölmeler oluşturur)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Bölmeler koleksiyonunu alın
            PaneCollection panes = worksheet.GetPanes();
            
            // Alt bölmenin ilk görünen satırını ayarlayın
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Alt bölmenin ilk görünen satırını çıktı olarak verin
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Çalışma kitabını kaydedin
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


