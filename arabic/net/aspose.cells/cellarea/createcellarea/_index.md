---
title: "CellArea.CreateCellArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CellArea. تنشئ مساحة خلية"
type: docs
url: /ar/net/aspose.cells/cellarea/createcellarea/
---
## CreateCellArea(int, int, int, int) {#createcellarea}

ينشئ مساحة خلية.

```csharp
public static CellArea CreateCellArea(int startRow, int startColumn, int endRow, int endColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | صف البداية. |
| startColumn | Int32 | عمود البداية. |
| endRow | Int32 | صف النهاية. |
| endColumn | Int32 | عمود النهاية. |

### قيمة الإرجاع

إرجاع [`CellArea`](../).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // املأ الخلايا ببيانات تجريبية
            int[] values = { 1, 3, 2, 6, 4, 5, 8, 9, 7 };
            for (int i = 0; i < values.Length; i++)
            {
                cells[i, i / 3].PutValue(values[i]);
            }

            // إنشاء وتكوين مُرتّب البيانات
            DataSorter sorter = wb.DataSorter;
            sorter.Clear();
            sorter.Order1 = SortOrder.Ascending;
            sorter.Key1 = 2;
            sorter.Order2 = SortOrder.Ascending;
            sorter.Key2 = 1;
            sorter.Order3 = SortOrder.Ascending;
            sorter.Key3 = 0;

            // فرز باستخدام CreateCellArea مع معلمات Int32
            sorter.Sort(cells, CellArea.CreateCellArea(0, 0, 8, 2));

            // أخرج القيم المرتبة
            Console.WriteLine("Sorted values:");
            for (int i = 0; i < 9; i++)
            {
                Console.WriteLine(cells[i, 2 - i / 3].IntValue);
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateCellArea(string, string) {#createcellarea_1}

ينشئ مساحة خلية.

```csharp
public static CellArea CreateCellArea(string startCellName, string endCellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startCellName | String | الخلية العلوية اليسرى للنطاق. |
| endCellName | String | الخلية السفلية اليمنى للنطاق. |

### قيمة الإرجاع

إرجاع [`CellArea`](../).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellAreaMethodCreateCellAreaWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // ملء بعض البيانات في العمود A
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue($"Data {i}");
            }

            // إنشاء نطاق خلايا من B1 إلى B10
            CellArea area = CellArea.CreateCellArea("B1", "B10");
            
            // إدراج نطاق مع إزاحة الخلايا إلى الأسفل
            cells.InsertRange(area, ShiftType.Down);
            
            // تحقق من العملية عن طريق فحص قيم الخلايا
            Console.WriteLine("Inserted range from B1 to B10. Total rows: " + cells.Rows.Count);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


