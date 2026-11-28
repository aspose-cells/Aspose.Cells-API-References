---
title: "Worksheet.GetPanes"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet yöntemi. Pencere bölmelerini alır"
type: docs
url: /tr/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Pencere bölmelerini alır.

```csharp
public PaneCollection GetPanes()
```

### Açıklamalar

Pencere bölünmemiş veya dondurulmamışsa.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 5. satır ve 3. sütunda bölmeleri dondurun
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Bölme bilgilerini al
            PaneCollection panes = worksheet.GetPanes();
            
            // Bölme bilgilerini göster
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


