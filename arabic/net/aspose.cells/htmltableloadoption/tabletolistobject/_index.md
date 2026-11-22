---
title: "HtmlTableLoadOption.TableToListObject"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlTableLoadOption. تشير إلى ما إذا كان سيتم إنشاء كائنات قائمة من الجدول المستورد. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmltableloadoption/tabletolistobject/
---
## HtmlTableLoadOption.TableToListObject property

يشير إلى ما إذا كان سيتم إنشاء كائنات قائمة من الجدول المستورد. القيمة الافتراضية هي false.

```csharp
public bool TableToListObject { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlTableLoadOptionPropertyTableToListObjectDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();

            // إنشاء خيارات تحميل HTML مع تمكين TableToListObject
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();
            HtmlTableLoadOption tableLoadOption = new HtmlTableLoadOption
            {
                TableIndex = 0,
                TableToListObject = true
            };
            loadOptions.TableLoadOptions.Add(tableLoadOption);

            // تحميل HTML مع الخيارات المحددة
            workbook = new Workbook("input.html", loadOptions);

            // حفظ كملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlTableLoadOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


