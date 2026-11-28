---
title: "ListBox.SelectedIndex"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBox özelliği. Bir liste kutusu veya combo kutusunda şu anda seçili öğenin indeks numarasını alır veya ayarlar. Sıfır tabanlı"
type: docs
url: /tr/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Liste kutusunda veya combo kutusunda şu anda seçili öğenin dizin numarasını alır veya ayarlar. Sıfır tabanlı.

```csharp
public int SelectedIndex { get; set; }
```

### Açıklamalar

-1 presents no item is selected.

### Örnekler

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


