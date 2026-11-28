---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Bir ComboBox veya ListBox için Value özelliğinin, MultiSelect özelliğinin fmMultiSelectSingle değerinde nasıl belirlendiğini temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

MultiSelect özelliği değeri (fmMultiSelectSingle) olduğunda bir ComboBox veya ListBox için Value özelliğinin nasıl belirlendiğini temsil eder.

```csharp
public int BoundColumn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // ListBox ActiveX kontrolü ekle
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // ListBox özelliklerini yapılandır
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // BoundColumn değerini 0 (ID sütunu) olarak ayarlayın - bu, bir öğe seçildiğinde döndürülecek değerdir.
            listBox.BoundColumn = 0;
            
            // TextColumn değerini 1 (Ad sütunu) olarak ayarlayın - bu, listede görüntülenecektir.
            listBox.TextColumn = 1;

            // Çalışma kitabını kaydedin
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


