---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cells. تشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان"
type: docs
url: /ar/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

يشير إلى أن ارتفاع الصف وارتفاع الخط الافتراضي متطابقان

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // تعيين وإظهار خاصية IsDefaultRowHeightMatched
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // احفظ المصنف
            workbook.Save("output.xlsx");

            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


