---
title: "Workbook.Protect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تحمي دفتر عمل"
type: docs
url: /ar/net/aspose.cells/workbook/protect/
---
## Workbook.Protect method

يحمي مصنفًا.

```csharp
public void Protect(ProtectionType protectionType, string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| protectionType | ProtectionType | نوع الحماية. |
| كلمة المرور | String | كلمة المرور لحماية دفتر العمل. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodProtectWithProtectionTypeStringDemo
    {
        public static void Run()
        {
            Workbook wbk = new Workbook();
            wbk.Protect(ProtectionType.Structure, "password123");
            
            wbk.Save("protected_workbook.xlsx", SaveFormat.Xlsx);
            wbk.Dispose();
        }
    }
}
```

### انظر أيضًا

* enum [ProtectionType](../../protectiontype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


