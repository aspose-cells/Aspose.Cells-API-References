---
title: "TextBoxCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextBoxCollection. تُضيف مربع نص إلى المجموعة"
type: docs
url: /ar/net/aspose.cells.drawing/textboxcollection/add/
---
## TextBoxCollection.Add method

يضيف مربع نص إلى المجموعة.

```csharp
public int Add(int topRow, int leftColumn, int height, int width)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| الارتفاع | Int32 | ارتفاع مربع النص، بوحدة البكسل. |
| العرض | Int32 | عرض مربع النص، بوحدة البكسل. |

### قيمة الإرجاع

[`TextBox`](../../textbox/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodAddWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int index = worksheet.TextBoxes.Add(1, 1, 50, 100);
            Console.WriteLine("TextBox added at index: " + index);
        }
    }
}
```

### انظر أيضًا

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


