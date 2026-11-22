---
title: "Cells.ClearRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تمسح المحتويات والتنسيق لنطاق"
type: docs
url: /ar/net/aspose.cells/cells/clearrange/
---
## ClearRange(CellArea) {#clearrange}

يمسح محتويات وتنسيق نطاق.

```csharp
public void ClearRange(CellArea range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نطاق | CellArea | النطاق الذي سيُمسح. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // املأ الخلايا ببيانات تجريبية
            for (int row = 0; row <= 2; row++)
            {
                for (int col = 0; col <= 2; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data_{row}_{col}";
                }
            }

            // حدد CellArea للمسح (الصفوف 0-2، الأعمدة 0-2)
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 0;
            clearArea.EndRow = 2;
            clearArea.StartColumn = 0;
            clearArea.EndColumn = 2;

            try
            {
                // امسح النطاق المحدد
                worksheet.Cells.ClearRange(clearArea);
                Console.WriteLine("Cleared cells in range: Rows 0-2, Columns 0-2");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearRange method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("CellsMethodClearRangeWithCellAreaDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearRange(int, int, int, int) {#clearrange_1}

يمسح محتويات وتنسيق نطاق.

```csharp
public void ClearRange(int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| endColumn | Int32 | فهرس العمود النهائي. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodClearRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // املأ بعض بيانات الاختبار
            cells[0, 0].PutValue(1);
            cells[0, 16383].PutValue(2);
            cells[1048575, 0].PutValue(3);
            cells[1048575, 16383].PutValue(4);

            // امسح نطاق ورقة العمل بالكامل
            cells.ClearRange(0, 0, 1048575, 16383);

            // احفظ المصنف
            workbook.Save("ClearRangeDemo.xlsx");

            Console.WriteLine("ClearRange demo executed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


