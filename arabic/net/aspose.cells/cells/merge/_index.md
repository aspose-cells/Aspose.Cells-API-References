---
title: "Cells.Merge"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تقوم بدمج نطاق محدد من الخلايا في خلية واحدة"
type: docs
url: /ar/net/aspose.cells/cells/merge/
---
## Merge(int, int, int, int) {#merge}

يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من هذا النطاق (مؤشر صفر) |
| firstColumn | Int32 | العمود الأول من هذا النطاق (مؤشر صفر) |
| totalRows | Int32 | عدد الصفوف (مؤشر واحد) |
| totalColumns | Int32 | عدد الأعمدة (مؤشر واحد) |

### ملاحظات

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضع قيمًا في الخلايا لتوضيح الدمج
            cells[0, 0].PutValue("Merged Area");
            cells[5, 5].PutValue("Not Merged");

            // دمج الخلايا بدءًا من الصف 0، العمود 0، ممتدة على 3 صفوف وعمودين
            cells.Merge(0, 0, 3, 2);

            // احفظ المصنف
            workbook.Save("MergeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool) {#merge_1}

يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool mergeConflict)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من هذا النطاق (مؤشر صفر) |
| firstColumn | Int32 | العمود الأول من هذا النطاق (مؤشر صفر) |
| totalRows | Int32 | عدد الصفوف (مؤشر واحد) |
| totalColumns | Int32 | عدد الأعمدة (مؤشر واحد) |
| mergeConflict | منطقي | نطاقات مدمجة متعارضة. |

### ملاحظات

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق. إذا كان mergeConflict صحيحًا وتعارض النطاق المدمج مع خلايا مدمجة أخرى، فسيتم إزالة الخلايا المدمجة الأخرى تلقائيًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // دمج الخلايا من الصف 3، العمود 4 (D3) إلى الصف 7، العمود 5 (E7) - 5 صفوف وعمودين
            worksheet.Cells.Merge(3, 4, 5, 2, true);
            
            // احفظ المصنف
            workbook.Save("MergeDemoOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Merge(int, int, int, int, bool, bool) {#merge_2}

يدمج نطاقًا محددًا من الخلايا في خلية واحدة.

```csharp
public void Merge(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool checkConflict, bool mergeConflict)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من هذا النطاق (مؤشر صفر) |
| firstColumn | Int32 | العمود الأول من هذا النطاق (مؤشر صفر) |
| totalRows | Int32 | عدد الصفوف (مؤشر واحد) |
| totalColumns | Int32 | عدد الأعمدة (مؤشر واحد) |
| checkConflict | منطقي | يشير إلى ما إذا كان فحص تداخل الخلايا المدمجة مع خلايا مدمجة أخرى |
| mergeConflict | منطقي | نطاقات مدمجة متعارضة. |

### ملاحظات

الإشارة إلى الخلية المدمجة عبر عنوان الخلية العليا اليسرى في النطاق. إذا كان mergeConflict صحيحًا وتعارض النطاق المدمج مع خلايا مدمجة أخرى، فسيتم إزالة الخلايا المدمجة الأخرى تلقائيًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodMergeWithInt32Int32Int32Int32BooleanBooDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ضع بعض البيانات في الخلايا لتتم دمجها
            cells[0, 1].PutValue("Merged Cell");
            cells[1, 1].PutValue("This will be merged");

            // دمج الخلايا بدون خيارات (دمج بسيط)
            cells.Merge(0, 1, 2, 2);
            Console.WriteLine("Cells merged without options");

            // قم بفك الدمج أولاً لتوضيح الدمج التالي
            cells.UnMerge(0, 1, 2, 2);

            // دمج الخلايا مع ignoreStyle=false و mergeConflict=true
            cells.Merge(0, 1, 2, 2, false, true);
            Console.WriteLine("Cells merged with ignoreStyle=false and mergeConflict=true");

            // احفظ المصنف
            workbook.Save("MergeCellsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


