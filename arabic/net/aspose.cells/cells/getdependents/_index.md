---
title: "Cells.GetDependents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. الحصول على جميع الخلايا التي تشير إلى الخلية المحددة"
type: docs
url: /ar/net/aspose.cells/cells/getdependents/
---
## Cells.GetDependents method

احصل على جميع الخلايا التي تشير إلى الخلية المحددة.

```csharp
public Cell[] GetDependents(bool isAll, int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isAll | منطقي | يشير إلى ما إذا كان يتم فحص أوراق العمل الأخرى |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetDependentsWithBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إعداد صيغ وعينات قيم
            cells["A1"].PutValue(10);
            cells["B1"].Formula = "=A1*2";
            cells["C1"].Formula = "=A1+B1";
            cells["D1"].Formula = "=B1*3";
            cells["F4"].Formula = "=A1*5";

            // حساب الصيغ
            workbook.CalculateFormula();

            // الحصول على التبعيات المباشرة للخلية A1 (الصف 0، العمود 0)
            Cell[] directDependents = cells.GetDependents(false, 0, 0);
            Console.WriteLine("Direct dependents of A1:");
            foreach (Cell cell in directDependents)
            {
                Console.WriteLine(cell.Name);
            }

            // الحصول على جميع التبعيات (بما في ذلك غير المباشرة) للخلية A1 (الصف 0، العمود 0)
            Cell[] allDependents = cells.GetDependents(true, 0, 0);
            Console.WriteLine("\nAll dependents of A1:");
            foreach (Cell cell in allDependents)
            {
                Console.WriteLine(cell.Name);
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


