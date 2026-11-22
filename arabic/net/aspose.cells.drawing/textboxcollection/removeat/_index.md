---
title: "TextBoxCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextBoxCollection. تُزيل مربع نص من الملف"
type: docs
url: /ar/net/aspose.cells.drawing/textboxcollection/removeat/
---
## TextBoxCollection.RemoveAt method

أزل مربع نص من الملف.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس مربع النص. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض مربعات النص إلى ورقة العمل
            for (int i = 0; i < 3; i++)
            {
                worksheet.TextBoxes.Add(10, 10 + (i * 30), 200, 50);
                worksheet.TextBoxes[i].Text = "TextBox " + (i + 1);
            }

            Console.WriteLine("Before removal - TextBox count: " + worksheet.TextBoxes.Count);

            // أزل آخر مربع نص باستخدام RemoveAt مع معامل Int32
            int lastIndex = worksheet.TextBoxes.Count - 1;
            worksheet.TextBoxes.RemoveAt(lastIndex);

            Console.WriteLine("After removal - TextBox count: " + worksheet.TextBoxes.Count);
        }
    }
}
```

### انظر أيضًا

* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


