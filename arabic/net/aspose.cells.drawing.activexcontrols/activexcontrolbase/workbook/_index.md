---
title: "ActiveXControlBase.Workbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ActiveXControlBase. تحصل على كائن Workbook"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/
---
## ActiveXControlBase.Workbook property

يحصل على كائن `Workbook`.

```csharp
public Workbook Workbook { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBasePropertyWorkbookDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // إضافة عنصر تحكم ActiveX إلى ورقة العمل
                Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 30);
                CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

                // تعيين بعض الخصائص لجعل المثال ذا معنى
                checkBox.Caption = "Sample CheckBox";
                checkBox.IsAutoSize = true;

                // عرض خاصية Workbook (للقراءة فقط)
                Workbook controlWorkbook = checkBox.Workbook;
                Console.WriteLine("ActiveX Control Workbook reference obtained successfully.");
                Console.WriteLine("Workbook has " + controlWorkbook.Worksheets.Count + " worksheets.");

                // تحقق من أن مرجع المصنف هو نفسه المصنف الأصلي لدينا
                if (controlWorkbook == workbook)
                {
                    Console.WriteLine("The ActiveX control's Workbook property correctly references the parent workbook.");
                }

                // احفظ المصنف
                workbook.Save("ActiveXControlWorkbookDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../../../aspose.cells/workbook/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


