---
title: "HorizontalPageBreakCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة HorizontalPageBreakCollection. تضيف فاصل صفحة أفقي إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/horizontalpagebreakcollection/add/
---
## Add(int, int, int) {#add_2}

يضيف فاصل صفحة أفقي إلى المجموعة.

```csharp
public int Add(int row, int startColumn, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف، يبدأ من الصفر. |
| startColumn | Int32 | فهرس العمود الابتدائي، يبدأ من الصفر. |
| endColumn | Int32 | فهرس العمود النهائي، يبدأ من الصفر. |

### قيمة الإرجاع

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### ملاحظات

تُستخدم هذه الطريقة لإضافة فاصل صفحة أفقي داخل منطقة الطباعة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عرض طريقة Add مع معلمات (Int32, Int32, Int32)
            worksheet.HorizontalPageBreaks.Add(10, 1, 5);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int) {#add}

يضيف فاصل صفحة أفقي إلى المجموعة.

```csharp
public int Add(int row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | مؤشر صف الخلية، يبدأ من الصفر. |

### قيمة الإرجاع

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة فواصل صفحات أفقية باستخدام معلمة Int32
            worksheet.HorizontalPageBreaks.Add(5);
            worksheet.HorizontalPageBreaks.Add(10);
            
            workbook.Save("HorizontalPageBreakExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int) {#add_1}

يضيف فاصل صفحة أفقي إلى المجموعة.

```csharp
public int Add(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | مؤشر صف الخلية، يبدأ من الصفر. |
| عمود | Int32 | مؤشر عمود الخلية، يبدأ من الصفر. |

### قيمة الإرجاع

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية لإنشاء عدة صفوف
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }

            // إضافة فواصل صفحات أفقية في صفوف محددة
            worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
            worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
            worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29

            // احفظ المصنف
            workbook.Save("HorizontalPageBreaksDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_3}

يضيف فاصل صفحة أفقي إلى المجموعة.

```csharp
public int Add(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |

### قيمة الإرجاع

[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.

### ملاحظات

تم إضافة فاصل الصفحة في أعلى اليسار من الخلية. يرجى ضبط فاصل صفحة أفقي وفاصل صفحة عمودي في آنٍ واحد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة فاصل صفحة أفقي عند الصف 4 (D5 هو الصف 4 في الفهرس القائم على الصفر)
            worksheet.HorizontalPageBreaks.Add("D5");
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


