---
title: "WorkbookDesigner.ContainsVariables"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookDesigner. تشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/containsvariables/
---
## WorkbookDesigner.ContainsVariables property

تشير إلى ما إذا كانت ورقة العمل الأولى تحتوي على متغيرات مخصصة.

```csharp
[Obsolete("Use WorkbookDesigner.VariablesWorksheetName property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ContainsVariables { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية WorkbookDesigner.VariablesWorksheetName. سيتم إزالة هذه الخاصية بعد 3 أشهر منذ سبتمبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDesignerPropertyContainsVariablesDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إنشاء ورقة عمل نموذجية
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات لجعل المثال ذو معنى
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // إنشاء مثيل WorkbookDesigner
                WorkbookDesigner designer = new WorkbookDesigner(workbook);

                // عرض القيمة الحالية لخاصية ContainsVariables
                Console.WriteLine("Initial ContainsVariables value: " + designer.ContainsVariables);

                // تعيين خاصية ContainsVariables إلى true
                designer.ContainsVariables = true;

                // عرض القيمة المحدثة
                Console.WriteLine("Updated ContainsVariables value: " + designer.ContainsVariables);

                // حفظ النتيجة
                workbook.Save("ContainsVariablesDemo.xlsx");

                Console.WriteLine("ContainsVariables property has been demonstrated");
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

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


