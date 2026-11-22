---
title: "ComboBox.DropDownLines"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ComboBox. تحصل أو تعين عدد أسطر القائمة المعروضة في الجزء المنسدل من مربع السرد"
type: docs
url: /ar/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

يحصل أو يضبط عدد أسطر القائمة المعروضة في الجزء المنسدل من مربع التحرير.

```csharp
public int DropDownLines { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أنشئ ComboBox بالمعلمات الصحيحة
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // املأ خلايا ورقة العمل بالعناصر
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // اربط مربع السرد بقيم الخلايا
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


