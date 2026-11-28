---
title: "ScrollBarActiveXControl.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ScrollBarActiveXControl özelliği. ActiveX kontrolünün tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/scrollbaractivexcontrol/type/
---
## ScrollBarActiveXControl.Type property

ActiveX denetiminin türünü alır.

```csharp
public override ControlType Type { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ScrollBarActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Doğru parametrelerle bir ScrollBar ActiveX kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 1, 1, 100, 20, 0);
            ScrollBarActiveXControl scrollBar = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Type özelliğini kullanarak kontrol tipini kontrol et
            if (scrollBar.Type == ControlType.ScrollBar)
            {
                // ScrollBar'a özgü özellikleri ayarla
                scrollBar.Max = 100;
                scrollBar.Min = 0;
                scrollBar.Position = 50;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ScrollBarActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlType](../../controltype/)
* class [ScrollBarActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


