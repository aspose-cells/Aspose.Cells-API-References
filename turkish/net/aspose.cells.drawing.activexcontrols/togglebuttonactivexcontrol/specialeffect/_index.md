---
title: "ToggleButtonActiveXControl.SpecialEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ToggleButtonActiveXControl özelliği. Denetimin özel etkisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/togglebuttonactivexcontrol/specialeffect/
---
## ToggleButtonActiveXControl.SpecialEffect property

Denetimin özel efektini alır ve ayarlar.

```csharp
public ControlSpecialEffectType SpecialEffect { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ToggleButtonActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ToggleButton ActiveX kontrolü ekleyin
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 1, 1, 1, 1, 100, 30);
            ToggleButtonActiveXControl control = (ToggleButtonActiveXControl)shape.ActiveXControl;

            // SpecialEffect özelliğini ayarla
            control.SpecialEffect = ControlSpecialEffectType.Bump;

            // Çalışma kitabını kaydedin
            workbook.Save("ToggleButtonSpecialEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ToggleButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


