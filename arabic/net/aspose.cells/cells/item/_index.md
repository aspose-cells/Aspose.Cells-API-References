---
title: "Cells.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تحصل على عنصر Cell في فهرس الصف والعمود المحددين للخلية"
type: docs
url: /ar/net/aspose.cells/cells/item/
---
## Cells indexer (1 of 2)

يحصل على عنصر [`Cell`](../../cell/) في صف الخلية والعمود المحددين.

```csharp
public Cell this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### قيمة الإرجاع

كائن [`Cell`](../../cell/).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // استخدام خاصية Item للوصول إلى الخلايا وتعديلها
            cells[0, 0].PutValue("Hello");
            cells[1, 0].PutValue("World");
            
            // استخدام خاصية Style عبر Cells
            Style style1 = cells[0, 0].GetStyle();
            style1.Font.IsBold = true;
            cells[0, 0].SetStyle(style1);

            Style style2 = cells[1, 0].GetStyle();
            style2.Font.Color = System.Drawing.Color.Red;
            cells[1, 0].SetStyle(style2);

            // احفظ المصنف
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Cells indexer (2 of 2)

يحصل على عنصر [`Cell`](../../cell/) بالاسم المحدد للخلية.

```csharp
public Cell this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية، بما في ذلك حرف العمود ورقم الصف، على سبيل المثال A5. |

### قيمة الإرجاع

كائن [`Cell`](../../cell/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // تعيين القيم باستخدام خاصية Item
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            
            // تعيين القيم في نطاق باستخدام خاصية Item
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);
            
            // الوصول إلى خصائص الخلية وتعديلها باستخدام Item
            Cell cell = cells["B1"];
            Style style = cell.GetStyle();
            style.Font.IsBold = true;
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("CellsPropertyItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


