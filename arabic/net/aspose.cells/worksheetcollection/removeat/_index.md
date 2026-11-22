---
title: "WorksheetCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. يزيل العنصر بالاسم المحدد"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

يضبط الحجم المعروض عندما يُستخدم ملف دفتر العمل ككائن Ole.

```csharp
public void RemoveAt(string name)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم العنصر الذي سيتم إزالته. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // أضف بعض أوراق العمل
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // إضافة نطاق مسمى (ثابت)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // عرض طريقة RemoveAt مع معامل نصي
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // احفظ المصنف
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

يزيل العنصر عند فهرس محدد.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | قيمة الفهرس للعنصر الذي سيتم إزالته. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            
            // أضف بعض أوراق العمل
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // عرض عدد أوراق العمل الأصلي
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // إزالة ورقة العمل عند الفهرس 1 (الورقة الثانية)
            wb.Worksheets.RemoveAt(1);

            // عرض عدد أوراق العمل المحدث
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


