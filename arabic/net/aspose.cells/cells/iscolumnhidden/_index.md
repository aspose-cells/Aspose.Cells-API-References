---
title: "Cells.IsColumnHidden"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا"
type: docs
url: /ar/net/aspose.cells/cells/iscolumnhidden/
---
## Cells.IsColumnHidden method

يتحقق مما إذا كان العمود في الفهرس المحدد مخفيًا.

```csharp
public bool IsColumnHidden(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود |

### قيمة الإرجاع

صحيح إذا كان العمود مخفيًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodIsColumnHiddenWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // إخفاء العمود C (الفهرس 2)
            cells.HideColumn(2);
            
            // تحقق مما إذا كان العمود C مخفيًا
            bool isHidden = cells.IsColumnHidden(2);
            
            Console.WriteLine("Is column C (index 2) hidden? " + isHidden);
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


