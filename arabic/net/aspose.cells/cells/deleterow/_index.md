---
title: "Cells.DeleteRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحذف صفًا"
type: docs
url: /ar/net/aspose.cells/cells/deleterow/
---
## DeleteRow(int) {#deleterow}

يحذف صفًا.

```csharp
public void DeleteRow(int rowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف الذي سيُحذف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // عيّن صيغة مشتركة في الصف 66
            cells[65, 0].SetSharedFormula("=SUM(B10:B66)", 1, 6);

            // احذف الصف 9 (سيؤدي ذلك إلى رفع الصفوف للأعلى)
            cells.DeleteRow(9);

            // تحقق من تعديل الصيغة بعد حذف الصف
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}66 formula after deletion: {cells[64, i].Formula}");
            }

            // احذف الصفوف 60-61 (سيؤدي ذلك إلى رفع الصفوف للأعلى)
            cells.DeleteRows(59, 2);

            // تحقق من تعديل الصيغة بعد حذف الصفوف
            for (int i = 1; i < 7; i++)
            {
                char columnName = (char)('A' + i);
                Console.WriteLine($"Cell {columnName}64 formula after deletion: {cells[62, i].Formula}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## DeleteRow(int, bool) {#deleterow_1}

يحذف صفًا.

```csharp
public void DeleteRow(int rowIndex, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف الذي سيُحذف. |
| updateReference | منطقي | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteRowWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["A4"].PutValue("Cherry");

            Console.WriteLine("Original Data:");
            for (int i = 1; i <= 4; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            sheet.Cells.DeleteRow(2, true);

            Console.WriteLine("\nData After Deletion:");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine(sheet.Cells[$"A{i}"].Value);
            }

            workbook.Save("DeleteRowExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


