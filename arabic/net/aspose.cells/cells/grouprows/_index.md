---
title: "Cells.GroupRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. يجمع الصفوف"
type: docs
url: /ar/net/aspose.cells/cells/grouprows/
---
## GroupRows(int, int, bool) {#grouprows_1}

يقوم بتجميع الصفوف.

```csharp
public void GroupRows(int firstIndex, int lastIndex, bool isHidden)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس الصف الأول لتجميعه. |
| lastIndex | Int32 | فهرس الصف الأخير لتجميعه. |
| isHidden | منطقي | يحدد ما إذا كانت الصفوف المجمعة مخفية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // ملء بعض البيانات
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Group {i + 1}");
                for (int j = 1; j <= 5; j++)
                {
                    cells[i, j].PutValue($"Data {j}");
                }
            }

            // اجمع الصفوف من 1 إلى 5 (فهرس يبدأ من 0) وأخفها
            cells.GroupRows(1, 5, true);

            // عيّن صف الملخص أسفل المجموعة
            worksheet.Outline.SummaryRowBelow = false;

            // احفظ المصنف
            workbook.Save("GroupRowsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupRows(int, int) {#grouprows}

يقوم بتجميع الصفوف.

```csharp
public void GroupRows(int firstIndex, int lastIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس الصف الأول لتجميعه. |
| lastIndex | Int32 | فهرس الصف الأخير لتجميعه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupRowsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض بيانات العينة
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue("Row " + (i + 1));
            }

            // اجمع الصفوف من 2 إلى 5 (فهرس يبدأ من الصفر)
            cells.GroupRows(1, 4);

            // احفظ المصنف
            workbook.Save("GroupRowsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


