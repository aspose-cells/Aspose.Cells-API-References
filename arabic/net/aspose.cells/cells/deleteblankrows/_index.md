---
title: "Cells.DeleteBlankRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. حذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر"
type: docs
url: /ar/net/aspose.cells/cells/deleteblankrows/
---
## DeleteBlankRows() {#deleteblankrows}

احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو كائن آخر.

```csharp
public void DeleteBlankRows()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إضافة بعض البيانات مع صفوف فارغة
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue("Data1");
            cells["A4"].PutValue("Data2"); // Blank row at A3
            cells["A6"].PutValue("Data3"); // Blank row at A5

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i < 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // حذف الصفوف الفارغة
            cells.DeleteBlankRows();

            Console.WriteLine("\nAfter deleting blank rows:");
            for (int i = 0; i < cells.MaxDataRow + 1; i++)
            {
                Console.WriteLine($"Row {i + 1}: {cells[i, 0].StringValue}");
            }

            // احفظ المصنف
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteBlankRows(DeleteOptions) {#deleteblankrows_1}

احذف جميع الصفوف الفارغة التي لا تحتوي على أي بيانات أو بعض الكائنات الخاصة مثل التعليق المرئي، جدول محوري.

```csharp
public void DeleteBlankRows(DeleteOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | DeleteOptions | خيارات حذف النطاق. |

### ملاحظات

بالنسبة للصفوف الفارغة التي سيتم حذفها، ليس من الضروري فقط أن يكون [`IsBlank`](../../row/isblank/) صحيحًا، بل يجب أيضًا ألا يكون هناك أي تعليق مرئي معرف لأي خلية في تلك الصفوف، ولا جدول محوري يتقاطع نطاقه معها.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteBlankRowsWithDeleteOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بعض بيانات الاختبار مع صفوف فارغة
            sheet.Cells["A1"].PutValue("Data1");
            sheet.Cells["A3"].PutValue("Data2");
            sheet.Cells["A5"].PutValue("Data3");
            
            // إنشاء خيارات الحذف
            DeleteOptions options = new DeleteOptions();
            options.UpdateReference = true;
            
            // حذف الصفوف الفارغة
            sheet.Cells.DeleteBlankRows(options);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DeleteOptions](../../deleteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


