---
title: "CheckBoxActiveXControl.Type"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. ActiveX kontrolünün tipini alır"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/type/
---
## CheckBoxActiveXControl.Type property

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
    public class CheckBoxActiveXControlPropertyTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CheckBox ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Özellikleri ayarla
            checkBox.Caption = "Sample CheckBox";
            checkBox.GroupName = "Sheet1";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.UnChecked;
            checkBox.IsEnabled = true;

            // Type özelliğinin kullanımını gösterin.
            Console.WriteLine("Control Type: " + checkBox.Type); // Output: Control Type: CheckBox
            if (checkBox.Type == ControlType.CheckBox)
            {
                Console.WriteLine("This is a CheckBox control");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [ControlType](../../controltype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


