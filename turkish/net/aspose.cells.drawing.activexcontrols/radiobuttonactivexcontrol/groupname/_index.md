---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "RadioButtonActiveXControl özelliği. Grubun adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Grubun adını alır ve ayarlar.

```csharp
public string GroupName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İki RadioButton ActiveX kontrolü ekle
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Onların birbirini dışlamasını sağlamak için aynı grup adını ayarla
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Başlıkları ayarla
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Çalışma kitabını kaydedin
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


