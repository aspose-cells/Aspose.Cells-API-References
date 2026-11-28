---
title: "LabelActiveXControl.SpecialEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "LabelActiveXControl özelliği. Denetimin özel etkisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/specialeffect/
---
## LabelActiveXControl.SpecialEffect property

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
    public class LabelActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Tüm gerekli parametrelerle bir Label ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.Label, 
                1, 1, 100, 50,  // upperLeftRow, upperLeftColumn, height, width
                100, 50);       // heightInPx, widthInPx
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Temel özellikleri ayarlayın
            labelControl.Caption = "Sample Label";
            labelControl.IsWordWrapped = true;

            // SpecialEffect özelliğini gösterin
            labelControl.SpecialEffect = ControlSpecialEffectType.Raised;
            Console.WriteLine("SpecialEffect set to: " + labelControl.SpecialEffect);

            // SpecialEffect'i değiştir ve farkı göster
            labelControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            Console.WriteLine("SpecialEffect changed to: " + labelControl.SpecialEffect);

            // Çalışma kitabını kaydedin
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


