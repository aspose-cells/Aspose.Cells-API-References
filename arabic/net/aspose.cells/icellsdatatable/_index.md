---
title: "واجهة ICellsDataTable"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.ICellsDataTable. تمثل جدول بيانات"
type: docs
url: /ar/net/aspose.cells/icellsdatatable/
---
## ICellsDataTable interface

يمثل جدول البيانات.

```csharp
public interface ICellsDataTable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Columns](../../aspose.cells/icellsdatatable/columns/) { get; } | يحصل على أسماء الأعمدة. |
| [Count](../../aspose.cells/icellsdatatable/count/) { get; } | يحصل على عدد السجلات. -1 للعدد غير المعروف للسجلات. |
| [Item](../../aspose.cells/icellsdatatable/item/) { get; } | يحصل على البيانات المخزنة في العمود المحدد بالفهرس. (2 مؤشرات) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BeforeFirst](../../aspose.cells/icellsdatatable/beforefirst/)() | حرك المؤشر إلى مقدمة هذا الكائن، مباشرةً قبل الصف الأول. |
| [Next](../../aspose.cells/icellsdatatable/next/)() | يحرك المؤشر أسفل صف واحد من موقعه الحالي. |

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassICellsDataTableDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();

            ArrayList dataLists = new ArrayList();
            ArrayList list1 = new ArrayList();
            list1.AddRange(new object[] { "Name", "Age", "Gender" });
            ArrayList list2 = new ArrayList();
            list2.AddRange(new object[] { "Alice", 30, "Female" });
            ArrayList list3 = new ArrayList();
            list3.AddRange(new object[] { "Bob", 25, "Male" });
            ArrayList list4 = new ArrayList();
            list4.AddRange(new object[] { "Charlie", 35, "Male" });
            dataLists.Add(list1);
            dataLists.Add(list2);
            dataLists.Add(list3);
            dataLists.Add(list4);

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            Console.WriteLine("First worksheet A2 value: " + wb.Worksheets[0].Cells["A2"].StringValue);

            wb.Worksheets.Add();
            wb.Worksheets[1].Cells.ImportArrayList(dataLists, 0, 0, true);
            Console.WriteLine("Second worksheet A3 value: " + wb.Worksheets[1].Cells["A3"].StringValue);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


