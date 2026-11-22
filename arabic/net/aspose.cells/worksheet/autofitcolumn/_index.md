---
title: "Worksheet.AutoFitColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تضبط عرض العمود تلقائيًا"
type: docs
url: /ar/net/aspose.cells/worksheet/autofitcolumn/
---
## AutoFitColumn(int, int, int) {#autofitcolumn_1}

يضبط عرض العمود تلقائيًا.

```csharp
public void AutoFitColumn(int columnIndex, int firstRow, int lastRow)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |
| firstRow | Int32 | فهرس الصف الأول. |
| lastRow | Int32 | فهرس الصف الأخير. |

### ملاحظات

هذه الطريقة تضبط الصف تلقائيًا بناءً على المحتوى في نطاق من الخلايا داخل الصف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetMethodAutoFitColumnWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ الخلايا ببيانات تجريبية تتطلب تعديل عرض العمود
            worksheet.Cells["A1"].PutValue("Short text");
            worksheet.Cells["A2"].PutValue("This is a much longer piece of text that will require column width adjustment");
            worksheet.Cells["A3"].PutValue("Another long text entry to demonstrate AutoFitColumn");
            
            try
            {

                Console.WriteLine($"Column width before: {worksheet.Cells.GetColumnWidth(0)}");
                // استدعِ AutoFitColumn على العمود A (الفهرس 0) للصفوف من 0 إلى 2 (صفرية الأساس)
                worksheet.AutoFitColumn(0, 0, 2);
                
                Console.WriteLine("AutoFitColumn method executed successfully on column A for rows 1-3");
                
                // اعرض التأثير عن طريق إظهار عرض العمود قبل وبعد
                Console.WriteLine($"Column width after: {worksheet.Cells.GetColumnWidth(0)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AutoFitColumn method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("AutoFitColumnWithInt32Int32Int32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AutoFitColumn(int) {#autofitcolumn}

يضبط عرض العمود تلقائيًا.

```csharp
public void AutoFitColumn(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |

### ملاحظات

AutoFitColumn هي دالة غير دقيقة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodAutoFitColumnWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات عينة إلى الخلايا في العمود 4 (فهرس يبدأ من 0)
            worksheet.Cells["D1"].PutValue("This is a test");
            worksheet.Cells["D2"].PutValue("AutoFitColumn demonstration");
            worksheet.Cells["D3"].PutValue("Aspose.Cells for .NET");
            
            // ضبط تلقائي للعمود 4 (فهرس يبدأ من 0)
            worksheet.AutoFitColumn(3);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


