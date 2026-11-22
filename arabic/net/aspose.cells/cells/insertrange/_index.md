---
title: "Cells.InsertRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُدرج نطاقًا من الخلايا وتُحرك الخلايا وفقًا لخيار الإزاحة"
type: docs
url: /ar/net/aspose.cells/cells/insertrange/
---
## InsertRange(CellArea, int, ShiftType, bool) {#insertrange_2}

يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | CellArea | منطقة الإزاحة. |
| shiftNumber | Int32 | عدد الصفوف أو الأعمدة التي سيتم إدراجها. |
| shiftType | ShiftType | خيار إزاحة الخلايا. |
| updateReference | منطقي | يشير إلى ما إذا كان سيتم تحديث المراجع في أوراق العمل الأخرى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض بيانات العينة
            cells["A1"].PutValue("Header");
            cells["A2"].PutValue(100);
            cells["A3"].PutValue(200);

            // حدد المنطقة لإدراجها (الصفوف 2-3، العمود A)
            CellArea area = CellArea.CreateCellArea(1, 0, 2, 0);

            // إدراج نطاق مع إزاحة الخلايا إلى اليمين وتحديث المراجع
            cells.InsertRange(area, 1, ShiftType.Right, true);

            // تحقق من العملية عن طريق فحص القيم
            Console.WriteLine("A2 value after insert: " + cells["A2"].StringValue);
            Console.WriteLine("B2 value after insert: " + cells["B2"].StringValue);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, ShiftType) {#insertrange}

يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

```csharp
public void InsertRange(CellArea area, ShiftType shiftType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | CellArea | منطقة الإزاحة. |
| shiftType | ShiftType | خيار إزاحة الخلايا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaShiftTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض البيانات التجريبية
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"R{row}C{col}");
                }
            }

            // حدد منطقة الخلية لإدراجها
            CellArea area = new CellArea();
            area.StartRow = 2;
            area.EndRow = 4;
            area.StartColumn = 1;
            area.EndColumn = 3;

            // إدراج نطاق وإزاحة الخلايا إلى الأسفل
            cells.InsertRange(area, ShiftType.Down);

            // احفظ المصنف
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertRange(CellArea, int, ShiftType) {#insertrange_1}

يدرج نطاقًا من الخلايا ويُحرك الخلايا وفقًا لخيار التحريك.

```csharp
public void InsertRange(CellArea area, int shiftNumber, ShiftType shiftType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | CellArea | منطقة الإزاحة. |
| shiftNumber | Int32 | عدد الصفوف أو الأعمدة التي سيتم إدراجها. |
| shiftType | ShiftType | خيار إزاحة الخلايا. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertRangeWithCellAreaInt32ShiftTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Original Data");
            worksheet.Cells["B1"].PutValue(100);
            worksheet.Cells["C1"].PutValue(200);
            
            // حدد منطقة الخلية لإدراجها (خلية واحدة B1)
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 0;
            area.StartColumn = 1;
            area.EndColumn = 1;
            
            // إدراج نطاق مع إزاحة الخلايا إلى اليمين
            worksheet.Cells.InsertRange(area, 1, ShiftType.Right);
            
            // احفظ المصنف
            workbook.Save("InsertRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


