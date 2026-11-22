---
title: "Cells.CreateRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تنشئ كائن Range من نطاق من الخلايا"
type: docs
url: /ar/net/aspose.cells/cells/createrange/
---
## CreateRange(string, string) {#createrange_3}

ينشئ كائن [`Range`](../../range/) من نطاق من الخلايا.

```csharp
public Range CreateRange(string upperLeftCell, string lowerRightCell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| upperLeftCell | String | اسم الخلية العلوية اليسرى. |
| lowerRightCell | String | اسم الخلية السفلية اليمنى. |

### قيمة الإرجاع

كائن [`Range`](../../range/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // إنشاء نطاق من A1 إلى A2
            Aspose.Cells.Range range = cells.CreateRange("A1", "A2");
            range.Name = "MyRange";
            
            // تعيين القيم في النطاق
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            
            // استخدام النطاق في صيغة
            cells["B1"].Formula = "=SUM(MyRange)";
            
            // احسب الصيغة
            workbook.CalculateFormula();
            
            Console.WriteLine("Sum of MyRange (A1:A2) is: " + cells["B1"].IntValue);
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, int, int) {#createrange_1}

ينشئ كائن [`Range`](../../range/) من نطاق من الخلايا.

```csharp
public Range CreateRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | الصف الأول من هذا النطاق |
| firstColumn | Int32 | العمود الأول من هذا النطاق |
| totalRows | Int32 | عدد الصفوف |
| totalColumns | Int32 | عدد الأعمدة |

### قيمة الإرجاع

كائن [`Range`](../../range/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نطاق المصدر (بدءًا من الصف 2، العمود 2 مع 3 صفوف و4 أعمدة)
            Aspose.Cells.Range rangeSrc = cells.CreateRange(2, 2, 3, 4);

            // املأ نطاق المصدر ببيانات عينة
            for (int i = 0; i < rangeSrc.RowCount; i++)
            {
                for (int j = 0; j < rangeSrc.ColumnCount; j++)
                {
                    rangeSrc[i, j].PutValue($"Data {i},{j}");
                }
            }

            // إنشاء نطاق الوجهة (بدءًا من الصف 8، العمود 0 بنفس الأبعاد)
            Aspose.Cells.Range rangeDest = cells.CreateRange(8, 0, 3, 4);

            // نسخ القيم من المصدر إلى الوجهة
            rangeDest.CopyValue(rangeSrc);

            // احفظ المصنف
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(string) {#createrange_2}

ينشئ كائن [`Range`](../../range/) من عنوان النطاق.

```csharp
public Range CreateRange(string address)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| address | String | عنوان النطاق. |

### قيمة الإرجاع

كائن [`Range`](../../range/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق باستخدام عنوان نصي
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2:D4");

            // ملء البيانات في النطاق
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Cell {i},{j}");
                }
            }

            // إنشاء نطاق آخر في ورقة عمل جديدة
            workbook.Worksheets.Add();
            Worksheet worksheet2 = workbook.Worksheets[1];
            Aspose.Cells.Range range2 = worksheet2.Cells.CreateRange("A1:C3");

            // نسخ البيانات بين النطاقات
            range2.Copy(range);

            // احفظ المصنف
            workbook.Save("CreateRangeWithStringDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateRange(int, int, bool) {#createrange}

ينشئ كائن [`Range`](../../range/) من صفوف الخلايا أو أعمدة الخلايا.

```csharp
public Range CreateRange(int firstIndex, int number, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | Int32 | فهرس الصف الأول أو فهرس العمود الأول، يبدأ من الصفر. |
| عدد | Int32 | إجمالي عدد الصفوف أو الأعمدة، يبدأ من الواحد. |
| isVertical | منطقي | صحيح - النطاق تم إنشاؤه من أعمدة الخلايا. خطأ - النطاق تم إنشاؤه من صفوف الخلايا. |

### قيمة الإرجاع

كائن [`Range`](../../range/).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCreateRangeWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إنشاء نطاق يبدأ من الخلية A1 (0,0) مع 5 صفوف و3 أعمدة
            Aspose.Cells.Range range = cells.CreateRange(0, 0, true);

            // ملء بعض البيانات في النطاق
            for (int i = 0; i < range.RowCount; i++)
            {
                for (int j = 0; j < range.ColumnCount; j++)
                {
                    range[i, j].PutValue($"Row {i}, Col {j}");
                }
            }

            // احفظ المصنف
            workbook.Save("CreateRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


