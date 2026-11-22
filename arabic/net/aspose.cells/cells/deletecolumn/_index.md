---
title: "Cells.DeleteColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحذف عمودًا"
type: docs
url: /ar/net/aspose.cells/cells/deletecolumn/
---
## DeleteColumn(int, bool) {#deletecolumn_1}

يحذف عمودًا.

```csharp
public void DeleteColumn(int columnIndex, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | مؤشر العمود الذي سيتم حذفه. |
| updateReference | منطقي | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // املأ بعض البيانات النموذجية في الخلايا
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }
            
            Console.WriteLine("Before deleting column:");
            PrintCellValues(sheet);
            
            // احذف العمود الأول وحرك الأعمدة المتبقية إلى اليسار
            sheet.Cells.DeleteColumn(0, true);
            
            Console.WriteLine("\nAfter deleting column 0:");
            PrintCellValues(sheet);
            
            // احفظ المصنف
            workbook.Save("DeleteColumnDemo.xlsx");
        }
        
        private static void PrintCellValues(Worksheet sheet)
        {
            for (int i = 0; i < 5; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    Console.Write(sheet.Cells[i, j].Value + "\t");
                }
                Console.WriteLine();
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

## DeleteColumn(int) {#deletecolumn}

يحذف عمودًا.

```csharp
public void DeleteColumn(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | مؤشر العمود الذي سيتم حذفه. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodDeleteColumnWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // املأ بعض البيانات النموذجية في الأعمدة
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // احذف العمود عند الفهرس 1 (العمود B)
            cells.DeleteColumn(1);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Column deleted successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


