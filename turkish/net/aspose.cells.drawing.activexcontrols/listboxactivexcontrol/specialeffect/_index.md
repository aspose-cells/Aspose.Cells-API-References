---
title: "ListBoxActiveXControl.SpecialEffect"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Kontrolün özel etkisini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/specialeffect/
---
## ListBoxActiveXControl.SpecialEffect property

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
    public class ListBoxActiveXControlPropertySpecialEffectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ListBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 1, 100, 100, 100, 100);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // SpecialEffect özelliğini ayarla
            listBox.SpecialEffect = ControlSpecialEffectType.Sunken;

            // SpecialEffect değerini doğrula ve çıktı ver
            Console.WriteLine("ListBox SpecialEffect: " + listBox.SpecialEffect);

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxSpecialEffectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlSpecialEffectType](../../controlspecialeffecttype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


