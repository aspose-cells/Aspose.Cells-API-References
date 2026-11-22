---
title: "ComboBox.SelectedCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBox. تحصل على الخلية المحددة في نطاق الإدخال الخاص بـ combo box"
type: docs
url: /ar/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

يحصل على الخلية المحددة في نطاق الإدخال لمربع التحرير.

```csharp
public Cell SelectedCell { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ComboBoxPropertySelectedCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء الخلايا ببيانات نموذجية لعناصر combobox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // إنشاء ComboBox وتعيين خصائصه
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // تعيين التحديد وعرض SelectedCell
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // تعديل قيمة الخلية المحددة
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // إظهار التأثير على الخلايا المجاورة
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


