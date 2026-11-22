---
title: "VbaProject.Protect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة VbaProject. تحمي أو تلغي حماية هذا مشروع VBA"
type: docs
url: /ar/net/aspose.cells.vba/vbaproject/protect/
---
## VbaProject.Protect method

يحمي أو يزيل الحماية عن مشروع VBA هذا.

```csharp
public void Protect(bool islockedForViewing, string password)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| islockedForViewing | منطقي | يشير إلى ما إذا كان يقفل المشروع للعرض. |
| كلمة المرور | String | إذا كانت القيمة null، يلغي حماية مشروع VBA هذا، وإلا يحمي مشروع VBA هذا. |

### ملاحظات

إذا كان islockedForViewing صحيحًا، لا يمكن أن تكون كلمة المرور null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaProjectMethodProtectWithBooleanStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف مع مشروع VBA
            Workbook workbook = new Workbook();
            workbook.VbaProject.Protect(false, "password123");
            
            // احفظ المصنف
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### انظر أيضًا

* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


