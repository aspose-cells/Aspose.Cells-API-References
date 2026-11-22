---
title: "WorkbookSettings.ProtectionType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل على نوع الحماية لدفتر العمل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/protectiontype/
---
## WorkbookSettings.ProtectionType property

يحصل على نوع الحماية للمصنف.

```csharp
public ProtectionType ProtectionType { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyProtectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // احمِ دفتر العمل بنوع الحماية Windows
            workbook.Protect(ProtectionType.Windows, "password123");
            
            // اعرض خاصية ProtectionType
            Console.WriteLine("Workbook protection type: " + workbook.Settings.ProtectionType);
            
            // احفظ المصنف
            workbook.Save("ProtectedWorkbook.xlsx");
            
            // حمّل دفتر العمل المحفوظ للتحقق من استمرار نوع الحماية
            Workbook loadedWorkbook = new Workbook("ProtectedWorkbook.xlsx");
            Console.WriteLine("Loaded workbook protection type: " + loadedWorkbook.Settings.ProtectionType);
        }
    }
}
```

### انظر أيضًا

* enum [ProtectionType](../../protectiontype/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


