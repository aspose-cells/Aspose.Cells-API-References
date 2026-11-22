---
title: "Cell.Characters"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تُرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية"
type: docs
url: /ar/net/aspose.cells/cell/characters/
---
## Cell.Characters method

يرجع كائن Characters الذي يمثل نطاقًا من الأحرف داخل نص الخلية.

```csharp
public FontSetting Characters(int startIndex, int length)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | Int32 | فهرس بداية الحرف. |
| الطول | Int32 | عدد الأحرف. |

### قيمة الإرجاع

كائن الأحرف.

### ملاحظات

هذه الطريقة تعمل فقط على الخلية التي تحتوي على قيمة نصية.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodCharactersWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["A1"].PutValue("Helloworld");
            cells["A1"].Characters(5, 5).Font.IsBold = true;
            cells["A1"].Characters(5, 5).Font.Color = Color.Blue;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../fontsetting/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


