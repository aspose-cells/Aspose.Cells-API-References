---
title: "ListBoxActiveXControl.Value"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Kontrolün değerini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Denetimin değerini alır ve ayarlar.

```csharp
public string Value { get; set; }
```

### Açıklamalar

Yalnızca [`SelectionType`](../selectiontype/) SelectionType.Single olduğunda etkili olur;

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ListBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Temel özellikleri ayarlayın
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Öğeleri Value özelliğini kullanarak ayarla
            listBox.Value = "Red;Green;Blue;Yellow";

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


