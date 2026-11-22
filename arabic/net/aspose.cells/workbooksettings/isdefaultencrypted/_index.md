---
title: "WorkbookSettings.IsDefaultEncrypted"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان تشفير الدفتر باستخدام كلمة مرور افتراضية إذا تم قفل الهيكل والنوافذ للدفتر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/isdefaultencrypted/
---
## WorkbookSettings.IsDefaultEncrypted property

يشير إلى ما إذا كان يتم تشفير المصنف باستخدام كلمة مرور افتراضية إذا تم قفل بنية المصنف والنوافذ.

```csharp
public bool IsDefaultEncrypted { get; set; }
```

### ملاحظات

القيمة الافتراضية الآن هي false. وهي نفس ما في MS Excel 2013.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsDefaultEncryptedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Console.WriteLine("IsDefaultEncrypted: " + workbook.Settings.IsDefaultEncrypted);
            
            workbook.Settings.IsDefaultEncrypted = true;
            Console.WriteLine("After setting to true: " + workbook.Settings.IsDefaultEncrypted);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


