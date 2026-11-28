---
title: "Enum ShowDropButtonType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Düşürme düğmesinin ne zaman gösterileceğini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Açılır düğmenin ne zaman gösterileceğini belirtir.

```csharp
public enum ShowDropButtonType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Never | `0` | Düşürme düğmesi asla gösterilmez. |
| Focus | `1` | Kontrol odaklandığında düşürme düğmesini göster. |
| Always | `2` | Düşürme düğmesi her zaman gösterilir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir ComboBox ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ComboBox ActiveX kontrolü için özellikleri ayarla
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // ComboBox'a bazı öğeler ekle
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Çalışma kitabını kaydedin
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


