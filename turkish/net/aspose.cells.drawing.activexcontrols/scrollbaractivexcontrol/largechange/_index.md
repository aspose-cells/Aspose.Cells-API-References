---
title: "ScrollBarActiveXControl.LargeChange"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBarActiveXControl özelliği. Position özelliğinin değiştiği miktarı alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/largechange/
---
## ScrollBarActiveXControl.LargeChange property

Position özelliğinin değiştiği miktarı alır ve ayarlar

```csharp
public int LargeChange { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyLargeChangeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ScrollBar ActiveX Kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 30);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // LargeChange özelliğini ayarla
            scrollBar.LargeChange = 5;

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarActiveXControlLargeChangeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


