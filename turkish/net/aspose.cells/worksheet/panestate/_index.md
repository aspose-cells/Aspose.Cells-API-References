---
title: "Worksheet.PaneState"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Bölmenin yatay veya dikey bölünmelere sahip olup olmadığını ve bu bölünmelerin dondurulup dondurulmadığını gösterir"
type: docs
url: /tr/net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Panelin yatay veya dikey bölünmeleri olup olmadığını ve bu bölünmelerin dondurulup dondurulmadığını gösterir.

```csharp
public PaneStateType PaneState { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyPaneStateDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");

            // Bölmeleri dondurun (ilk satır)
            worksheet.FreezePanes(1, 0, 1, 0);

            // Panel durumunu al ve görüntüle
            PaneStateType paneState = worksheet.PaneState;
            Console.WriteLine("Pane State: " + paneState);

            // Çalışma kitabını kaydet
            workbook.Save("PaneStateDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


