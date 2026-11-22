---
title: "Cells.EndCellInRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصل على الخلية الأخيرة في هذا الصف"
type: docs
url: /ar/net/aspose.cells/cells/endcellinrow/
---
## EndCellInRow(int) {#endcellinrow}

يحصل على الخلية الأخيرة في هذا الصف.

```csharp
public Cell EndCellInRow(int rowIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | Int32 | فهرس الصف. |

### قيمة الإرجاع

كائن الخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodEndCellInRowWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ البيانات في الصف 5 (فهرس يبدأ من الصفر)
            worksheet.Cells[5, 2].PutValue("Data1");
            worksheet.Cells[5, 4].PutValue("Data2");
            worksheet.Cells[5, 6].PutValue("Data3");

            try
            {
                // استدعِ EndCellInRow مع فهرس الصف 5
                Cell endCell = worksheet.Cells.EndCellInRow(5);
                
                if (endCell != null)
                {
                    Console.WriteLine($"Last cell in row 5: {endCell.Name}");
                    Console.WriteLine($"Cell value: {endCell.StringValue}");
                }
                else
                {
                    Console.WriteLine("No cells found in row 5");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing EndCellInRow: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellsMethodEndCellInRowWithInt32Demo.xlsx");
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

## EndCellInRow(int, int, int, int) {#endcellinrow_1}

يحصل على الخلية الأخيرة ذات أعلى فهرس صف في هذا النطاق.

```csharp
public Cell EndCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | فهرس الصف الابتدائي. |
| endRow | Int32 | فهرس الصف النهائي. |
| startColumn | Int32 | فهرس العمود الابتدائي. |
| endColumn | Int32 | فهرس العمود النهائي. |

### قيمة الإرجاع

كائن الخلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodEndCellInRowWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بعض البيانات في ورقة العمل
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Cell_{i}_{j}");
                }
            }

            // احصل على الخلية النهائية في الصف 3 بين العمودين 1 إلى 4
            Cell endCell = worksheet.Cells.EndCellInRow(3, 1, 3, 4);

            // اعرض مؤشرات الصف والعمود للخلية النهائية
            Console.WriteLine($"End cell in row 3 between columns 1-4 is at: Row {endCell.Row}, Column {endCell.Column}");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


