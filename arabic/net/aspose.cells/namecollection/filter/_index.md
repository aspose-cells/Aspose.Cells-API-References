---
title: "NameCollection.Filter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة NameCollection. تحصل على جميع الأسماء المعرفة حسب النطاق"
type: docs
url: /ar/net/aspose.cells/namecollection/filter/
---
## NameCollection.Filter method

يحصل على جميع الأسماء المعرفة حسب النطاق.

```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | NameScopeType | نوع النطاق. |
| sheetIndex | Int32 | فهرس الورقة. يؤثر فقط عندما يكون نوع النطاق Worksheet |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بعض الأسماء إلى المصنف وورقات العمل
            workbook.Worksheets.Names.Add("GlobalName");
            Worksheet worksheet1 = workbook.Worksheets[0];
            workbook.Worksheets.Names.Add("Sheet1Name");
            Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Names.Add("Sheet2Name");

            // تصفية الأسماء حسب نوع النطاق وفهرس الورقة
            Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
            Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
            Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);

            // إخراج النتائج
            Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
            Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
            Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
        }
    }
}
```

### انظر أيضًا

* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


