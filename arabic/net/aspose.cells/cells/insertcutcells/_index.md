---
title: "Cells.InsertCutCells"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. إدراج نطاق مقطوع"
type: docs
url: /ar/net/aspose.cells/cells/insertcutcells/
---
## Cells.InsertCutCells method

إدراج نطاق مقطوع.

```csharp
public void InsertCutCells(Range cutRange, int row, int column, ShiftType shiftType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cutRange | النطاق | نطاق القطع. |
| صف | Int32 | الصف. |
| عمود | Int32 | العمود. |
| shiftType | ShiftType | يشير إلى كيفية إزاحة الكائنات الأخرى للنطاق المستهدف عند إدراج نطاق القص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertCutCellsWithRangeInt32Int32ShiftTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وخلاياها
            Worksheet sourceSheet = workbook.Worksheets[0];
            Cells sourceCells = sourceSheet.Cells;
            
            // أضف بعض البيانات إلى الخلايا المصدر
            sourceCells["A1"].PutValue("Source A1");
            sourceCells["B1"].PutValue("Source B1");
            sourceCells["A2"].PutValue("Source A2");
            sourceCells["B2"].PutValue("Source B2");
            
            // أنشئ ورقة عمل ثانية كوجهة
            Worksheet destSheet = workbook.Worksheets.Add("Sheet2");
            Cells destCells = destSheet.Cells;
            
            // أضف بعض البيانات الأولية إلى الوجهة
            destCells["A1"].PutValue("Dest A1");
            destCells["B1"].PutValue("Dest B1");
            
            // أنشئ نطاقًا للقص (A1:B2 من ورقة المصدر)
            Aspose.Cells.Range cutRange = sourceCells.CreateRange("A1:B2");
            
            // أدرج الخلايا المقصوصة عند B2 في ورقة الوجهة، مع إزاحة الخلايا إلى الأسفل
            destCells.InsertCutCells(cutRange, 1, 1, ShiftType.Down);
            
            // احفظ المصنف
            workbook.Save("InsertCutCellsDemo.xlsx");
            
            Console.WriteLine("InsertCutCells demo executed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [Range](../../range/)
* enum [ShiftType](../../shifttype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


