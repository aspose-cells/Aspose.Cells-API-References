---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Sütun başlıklarının gösterilip gösterilmediğini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Sütun başlıklarının gösterilip gösterilmediğini belirtir.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Gerekli tüm parametrelerle bir ListBox ActiveX kontrolü ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // ListBox için özellikleri ayarla
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Örnek veri ekleyin
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


