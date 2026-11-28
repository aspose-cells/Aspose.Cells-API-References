---
title: "Worksheet.IsRulerVisible"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Cetvelin görünür olup olmadığını gösterir. Bu özellik yalnızca sayfa kırılımı önizlemesi için uygulanır."
type: docs
url: /tr/net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Cetvelin görünür olup olmadığını gösterir. Bu özellik yalnızca sayfa kesme önizlemesi için uygulanır.

```csharp
public bool IsRulerVisible { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyIsRulerVisibleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasını cetvelin görünür olduğu PageLayoutView moduna ayarla
            worksheet.ViewType = ViewType.PageLayoutView;

            // Cetvel görünürlüğünü değiştir
            worksheet.IsRulerVisible = true;

            // Mevcut cetvel görünürlük durumunu çıktı olarak ver
            Console.WriteLine("Worksheet ruler is visible: " + worksheet.IsRulerVisible);

            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetRulerVisibilityDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


