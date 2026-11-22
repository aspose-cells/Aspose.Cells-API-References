---
title: "WorksheetCollection.CreateUnionRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تنشئ كائن Range من عنوان النطاق"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/createunionrange/
---
## WorksheetCollection.CreateUnionRange method

ينشئ كائن [`Range`](../../range/) من عنوان النطاق.

```csharp
public UnionRange CreateUnionRange(string address, int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| address | String | عنوان النطاق. |
| sheetIndex | Int32 | فهرس الورقة. |

### قيمة الإرجاع

كائن [`Range`](../../range/)

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodCreateUnionRangeWithStringInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق موحد من سلاسل العناوين
            UnionRange unionRange = workbook.Worksheets.CreateUnionRange("A1:A5,B1:B5", 0);
            
            // تعيين قيمة للنطاق الاتحاد بالكامل
            unionRange.Value = "Test";
            
            // تطبيق التنسيق على النطاق الموحد
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Font.IsBold = true;
            unionRange.ApplyStyle(style, new StyleFlag { FontBold = true, FontColor = true });
            
            // احفظ المصنف
            workbook.Save("UnionRangeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [UnionRange](../../unionrange/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


