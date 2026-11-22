---
title: "WorkbookDesigner.LineByLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/linebyline/
---
## WorkbookDesigner.LineByLine property

تشير إلى ما إذا كان يتم معالجة العلامة الذكية سطرًا بسطر.

```csharp
[Obsolete("Use range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool LineByLine { get; set; }
```

### ملاحظات

القيمة الافتراضية هي true. إذا كانت False، يجب أن يحتوي ملف القالب على نطاق اسمه "_CellsSmartMarkers".

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام نطاق العلامات الذكية. سيتم إزالة هذه الخاصية بعد 12 شهرًا اعتبارًا من يوليو 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerPropertyLineByLineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل تجريبي مع العلامات الذكية
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // إعداد العلامات الذكية في ورقة العمل
            ws.Cells["A1"].PutValue("&RootData.Name");
            ws.Cells["A2"].PutValue("&RootData.Age");
            ws.Cells["A3"].PutValue("&RootData.Department");
            
            // إنشاء بيانات نموذجية
            var employee = new EmployeeData
            {
                Name = "John Doe",
                Age = 35,
                Department = "Sales"
            };
            
            List<EmployeeData> employees = new List<EmployeeData> { employee };

            // المعالجة مع LineByLine مضبوطة على false
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = wb,
                LineByLine = false // This is the key property being demonstrated
            };
            
            designer.SetDataSource("RootData", employees);
            designer.Process();

            // حفظ النتيجة
            wb.Save("output.xlsx");
            
            Console.WriteLine("Workbook processed with LineByLine=false. Output saved to output.xlsx");
        }
    }

    // فئة بيانات بسيطة للتوضيح
    public class EmployeeData
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public string Department { get; set; }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


