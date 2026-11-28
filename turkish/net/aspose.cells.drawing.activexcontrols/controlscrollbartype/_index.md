---
title: "Enum ControlScrollBarType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType enum. Kaydırma çubuğu türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Kaydırma çubuğunun türünü temsil eder.

```csharp
public enum ControlScrollBarType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Kaydırma çubuğu göstermez. |
| Horizontal | `1` | Yatay bir kaydırma çubuğu gösterir. |
| BarsVertical | `2` | Dikey bir kaydırma çubuğu gösterir. |
| BarsBoth | `3` | Hem yatay hem de dikey bir kaydırma çubuğu gösterir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir ListBox ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Hem yatay hem de dikey kaydırma çubuklarını göstermek için ScrollBars özelliğini ayarlayın
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Çalışma kitabını kaydedin
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


