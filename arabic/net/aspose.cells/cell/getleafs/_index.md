---
title: "Cell.GetLeafs"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. احصل على جميع الخلايا التي تشير إلى هذه الخلية مباشرة وتحتاج إلى التحديث عندما يتم تعديل هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

احصل على جميع الخلايا التي تشير إلى هذه الخلية مباشرة وتحتاج إلى التحديث عندما يتم تعديل هذه الخلية.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### قيمة الإرجاع

المعدِّد لتعداد جميع التابعين (Cell)

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.GetDependentsInCalculation(bool) للحصول على جميع التابعين في سلسلة الحساب. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات والصيغ لإنشاء تبعيات
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // احصل على الخلية التي لديها تابعين
                Cell cell = worksheet.Cells["B1"];

                // استدعِ GetLeafs للحصول على جميع الخلايا التي تشير إلى هذه الخلية مباشرة
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // احفظ المصنف
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

احصل على جميع الخلايا التي سيتم تحديثها عندما يتم تعديل هذه الخلية.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| recursive | منطقي | ما إذا كان يُعيد تلك leafs التي لا تشير إلى هذه الخلية مباشرة ولكنها تشير إلى leafs أخرى لهذه الخلية |

### قيمة الإرجاع

المعدِّد لتعداد جميع التابعين (Cell)

### ملاحظات

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام Cell.GetDependentsInCalculation(bool) للحصول على جميع التابعين في سلسلة الحساب. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مايو 2022. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات مع الصيغ لإنشاء تبعيات
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // احصل على الخلية التي لديها تابعين
                Cell cell = worksheet.Cells["A1"];

                // استدعِ GetLeafs مع تعيين المعامل المتكرر إلى true
                IEnumerator leafs = cell.GetLeafs(true);

                // عرض النتائج
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // احفظ المصنف
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


