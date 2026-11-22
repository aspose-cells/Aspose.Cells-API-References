---
title: "VerticalPageBreakCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VerticalPageBreakCollection. تضيف فاصل صفحة عمودي إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/verticalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

يضيف فاصل صفحة عمودي إلى المجموعة.

```csharp
public int Add(int startRow, int endRow, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس صف البداية، يبدأ من الصفر. |
| endRow | Int32 | فهرس صف النهاية، يبدأ من الصفر. |
| عمود | Int32 | فهرس العمود، يبدأ من الصفر. |

### قيمة الإرجاع

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### ملاحظات

يُستخدم هذا الأسلوب لإضافة فاصل صفحة عمودي داخل منطقة الطباعة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
            
            // عرض إضافة باستخدام معلمات (Int32, Int32, Int32)
            verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
            
            // أمثلة إضافية للسياق
            verticalPageBreaks.Add(4); // At column 4
            verticalPageBreaks.Add(5, 3); // At row 5, column 3

            Console.WriteLine("Vertical Page Breaks:");
            for (int i = 0; i < verticalPageBreaks.Count; i++)
            {
                VerticalPageBreak vpb = verticalPageBreaks[i];
                Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
            }

            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

يضيف فاصل صفحة عمودي إلى المجموعة.

```csharp
public int Add(int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | Int32 | مؤشر عمود الخلية، يبدأ من الصفر. |

### قيمة الإرجاع

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;

            // عرض طريقة الإضافة باستخدام معلمة Int32
            verticalPageBreaks.Add(4); // Add vertical page break at column 4

            // اطبع تفاصيل فاصل الصفحة المضاف
            VerticalPageBreak vpb = verticalPageBreaks[0];
            Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");

            workbook.Save("VerticalPageBreakCollectionExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

يضيف فاصل صفحة عمودي إلى المجموعة.

```csharp
public int Add(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | مؤشر صف الخلية، يبدأ من الصفر. |
| عمود | Int32 | مؤشر عمود الخلية، يبدأ من الصفر. |

### قيمة الإرجاع

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على مجموعة فواصل الصفحات العمودية
            VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;

            // أضف فواصل صفحات عمودية في مواضع أعمدة مختلفة
            vPageBreaks.Add(0, 5);  // Add page break after column 5
            vPageBreaks.Add(0, 10); // Add page break after column 10
            vPageBreaks.Add(0, 15); // Add page break after column 15

            // أضف بعض البيانات التجريبية لتصوير فواصل الصفحات
            for (int i = 0; i < 20; i++)
            {
                worksheet.Cells[0, i].PutValue($"Column {i + 1}");
            }

            // احفظ المصنف
            workbook.Save("VerticalPageBreaksDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

يضيف فاصل صفحة عمودي إلى المجموعة.

```csharp
public int Add(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |

### قيمة الإرجاع

[`VerticalPageBreak`](../../verticalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.VerticalPageBreaks.Add("G5");
            
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### انظر أيضًا

* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


