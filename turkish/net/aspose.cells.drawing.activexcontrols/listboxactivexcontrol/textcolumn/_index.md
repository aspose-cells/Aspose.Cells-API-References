---
title: "ListBoxActiveXControl.TextColumn"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListBoxActiveXControl özelliği. Kullanıcıya gösterilecek bir ComboBox veya ListBox'taki sütunu temsil eder."
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/textcolumn/
---
## ListBoxActiveXControl.TextColumn property

Kullanıcıya gösterilecek bir ComboBox veya ListBox'taki sütunu temsil eder.

```csharp
public int TextColumn { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyTextColumnDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // ListBox'u TextColumn özelliğiyle yapılandırın.
            listBox.ColumnCount = 2;
            listBox.TextColumn = 1; // Demonstrating TextColumn property
            listBox.ListFillRange = "A2:B5";

            // Örnek veri ekleyin (iki sütun).
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Description1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Description2");
            worksheet.Cells["A4"].PutValue("Item3");
            worksheet.Cells["B4"].PutValue("Description3");
            worksheet.Cells["A5"].PutValue("Item4");
            worksheet.Cells["B5"].PutValue("Description4");

            workbook.Save("ListBoxTextColumnDemo.xlsx");
            Console.WriteLine("ListBox with TextColumn demo created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


