---
title: "WorkbookSettings.Author"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. الحصول وتعيين مؤلف الملف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/author/
---
## WorkbookSettings.Author property

يحصل على مؤلف الملف ويضبطه.

```csharp
public string Author { get; set; }
```

### ملاحظات

لم يتم تعيينه، تحقق أولاً من [`Author`](../../../aspose.cells.properties/builtindocumentpropertycollection/author/)، ثم تحقق من مستخدم Environment.

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyAuthorDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى WorkbookSettings
            WorkbookSettings settings = workbook.Settings;

            // تعيين خاصية المؤلف
            settings.Author = "John Doe";

            // أضف بعض البيانات التجريبية لتوضيح وظائف المصنف
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Sample Workbook");
            sheet.Cells["A2"].PutValue("Created by: " + settings.Author);
            sheet.Cells["A3"].PutValue(DateTime.Now.ToString());

            // احفظ المصنف
            workbook.Save("AuthorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


