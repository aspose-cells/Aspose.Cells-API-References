---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PaneCollection özelliği. Sağ bölmenin ilk görünen sütununu alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Sağ bölmenin ilk görünen sütununu alır ve ayarlar.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Satır ve sütun indekslerini (5, 3) belirterek bölmeleri dondurun
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Bölmeler koleksiyonunu alın
            PaneCollection panes = sheet.GetPanes();
            
            // Sağ bölmenin ilk görünen sütununu ayarlayın
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


