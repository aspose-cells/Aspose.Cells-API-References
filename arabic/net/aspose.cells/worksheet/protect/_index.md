---
title: "Worksheet.Protect"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحمي ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/protect/
---
## Protect(ProtectionType) {#protect}

يحمي ورقة العمل.

```csharp
public void Protect(ProtectionType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ProtectionType | نوع الحماية. |

### ملاحظات

هذه الطريقة تحمي ورقة العمل بدون كلمة مرور. يمكنها حماية ورقة العمل في جميع إصدارات ملف Excel.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // حماية ورقة العمل بنوع الحماية Objects
            sheet.Protect(ProtectionType.Objects);
            
            // احفظ المصنف
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Protect(ProtectionType, string, string) {#protect_1}

يحمي ورقة العمل.

```csharp
public void Protect(ProtectionType type, string password, string oldPassword)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | ProtectionType | نوع الحماية. |
| كلمة المرور | String | كلمة المرور. |
| oldPassword | String | إذا كانت ورقة العمل محمية بالفعل بكلمة مرور، يرجى تقديم كلمة المرور القديمة. وإلا، يمكنك تعيين قيمة فارغة أو سلسلة فارغة لهذا المعامل. |

### ملاحظات

يمكن لهذه الطريقة حماية ورقة العمل في جميع إصدارات ملف Excel.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodProtectWithProtectionTypeStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احمِ ورقة العمل باستخدام كلمة مرور واسمح بجميع أنواع الحماية
            worksheet.Protect(ProtectionType.All, "password123", null);
            
            // احفظ المصنف
            workbook.Save("ProtectedWorksheet.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ProtectionType](../../protectiontype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


