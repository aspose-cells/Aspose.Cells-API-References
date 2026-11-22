---
title: "Cells.GroupColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تجمع الأعمدة"
type: docs
url: /ar/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

يقوم بتجميع الأعمدة.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس العمود الأول لتجميعه. |
| lastIndex | Int32 | فهرس العمود الأخير لتجميعه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تجميع الأعمدة من الفهرس 0 إلى 255
            cells.GroupColumns(0, 255);

            // احفظ المصنف
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

يقوم بتجميع الأعمدة.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس العمود الأول لتجميعه. |
| lastIndex | Int32 | فهرس العمود الأخير لتجميعه. |
| isHidden | منطقي | يحدد ما إذا كانت الأعمدة المجمعة مخفية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تجميع الأعمدة من 5 إلى 7 (3 أعمدة) وإخفاؤها
            cells.GroupColumns(5, 7, true);

            // احفظ المصنف
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


