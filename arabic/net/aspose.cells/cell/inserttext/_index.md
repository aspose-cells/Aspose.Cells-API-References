---
title: "Cell.InsertText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. إدراج بعض الأحرف إلى الخلية. إذا كانت الخلية ذات تنسيق غني، يمكن لهذه الطريقة الحفاظ على التنسيق الأصلي."
type: docs
url: /ar/net/aspose.cells/cell/inserttext/
---
## Cell.InsertText method

إدراج بعض الأحرف إلى الخلية. إذا كانت الخلية منسقة بنص غني، يمكن لهذه الطريقة الحفاظ على التنسيق الأصلي.

```csharp
public void InsertText(int index, string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس. |
| نص | String | نص مُدرج. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodInsertTextWithInt32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى الخلية B3 وتعيين القيمة الأولية
            Cell cell = worksheet.Cells["B3"];
            cell.PutValue("OriginalText");
            
            // إدراج نص في الموضع 6
            cell.InsertText(6, "Inserted");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


