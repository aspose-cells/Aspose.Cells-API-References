---
title: "ControlScrollOrientation enum'ı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation enum'ı. Kaydırma yönünün tipini temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Kaydırma yönünün türünü temsil eder.

```csharp
public enum ControlScrollOrientation
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Auto | `3` | Denetimin genişliği yüksekliğinden büyük olduğunda denetim yatay olarak işlenir. Aksi takdirde denetim dikey olarak işlenir. |
| Vertical | `0` | Denetim dikey olarak işlenir. |
| Horizontal | `1` | Denetim yatay olarak işlenir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            
            // İlk worksheet'e bir ScrollBarActiveXControl ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // ScrollBarActiveXControl için özellikleri ayarlayın
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // ControlScrollOrientation enum'ı kullanarak yön ayarlamayı gösterin
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


