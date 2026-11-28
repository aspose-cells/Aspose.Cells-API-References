---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CheckBoxActiveXControl özelliği. Grubun adını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Grubun adını alır ve ayarlar.

```csharp
public string GroupName { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // CheckBox ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // GroupName özelliğini ayarla
            checkBox.GroupName = "Sheet1";

            // GroupName'i doğrula ve çıktısını al
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Çalışma kitabını kaydedin
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


