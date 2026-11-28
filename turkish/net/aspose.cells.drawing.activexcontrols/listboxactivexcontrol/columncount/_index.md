---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Bir ComboBox veya ListBox'ta görüntülenecek sütun sayısını temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Bir ComboBox veya ListBox'ta görüntülenecek sütun sayısını temsil eder.

```csharp
public int ColumnCount { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir ListBox ActiveX kontrolü ekleyin
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // ColumnCount dahil olmak üzere özellikleri ayarlayın.
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // ColumnCount değerini doğrulayın ve çıktısını verin.
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

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


