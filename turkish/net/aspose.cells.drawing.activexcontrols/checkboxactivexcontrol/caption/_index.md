---
title: "CheckBoxActiveXControl.Caption"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. Kontrol üzerinde görünen açıklayıcı metni alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

Kontrol üzerinde görünen açıklayıcı metni alır ve ayarlar.

```csharp
public string Caption { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CheckBox ActiveX kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Caption özelliğini ayarla ve göster
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


