---
title: "الفئة Protection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Protection. تمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل"
type: docs
url: /ar/net/aspose.cells/protection/
---
## Protection class

يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل.

```csharp
public class Protection
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowDeletingColumn](../../aspose.cells/protection/allowdeletingcolumn/) { get; set; } | يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية. |
| [AllowDeletingRow](../../aspose.cells/protection/allowdeletingrow/) { get; set; } | يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية. |
| [AllowEditingContent](../../aspose.cells/protection/alloweditingcontent/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية. |
| [AllowEditingObject](../../aspose.cells/protection/alloweditingobject/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع كائنات الرسم في ورقة عمل محمية. |
| [AllowEditingScenario](../../aspose.cells/protection/alloweditingscenario/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بتحرير السيناريوهات في ورقة عمل محمية. |
| [AllowFiltering](../../aspose.cells/protection/allowfiltering/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم باستخدام الفلتر التلقائي الذي تم إنشاؤه قبل حماية الورقة. |
| [AllowFormattingCell](../../aspose.cells/protection/allowformattingcell/) { get; set; } | يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية. |
| [AllowFormattingColumn](../../aspose.cells/protection/allowformattingcolumn/) { get; set; } | يمثل ما إذا كان تنسيق الأعمدة مسموحًا به في ورقة عمل محمية. |
| [AllowFormattingRow](../../aspose.cells/protection/allowformattingrow/) { get; set; } | يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية. |
| [AllowInsertingColumn](../../aspose.cells/protection/allowinsertingcolumn/) { get; set; } | يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية. |
| [AllowInsertingHyperlink](../../aspose.cells/protection/allowinsertinghyperlink/) { get; set; } | يمثل ما إذا كان إدراج الروابط التشعبية مسموحًا به في ورقة عمل محمية. |
| [AllowInsertingRow](../../aspose.cells/protection/allowinsertingrow/) { get; set; } | يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية. |
| [AllowSelectingLockedCell](../../aspose.cells/protection/allowselectinglockedcell/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية. |
| [AllowSelectingUnlockedCell](../../aspose.cells/protection/allowselectingunlockedcell/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية. |
| [AllowSorting](../../aspose.cells/protection/allowsorting/) { get; set; } | يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية. |
| [AllowUsingPivotTable](../../aspose.cells/protection/allowusingpivottable/) { get; set; } | يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع جداول المحور في ورقة عمل محمية. |
| [IsProtectedWithPassword](../../aspose.cells/protection/isprotectedwithpassword/) { get; } | يشير إلى ما إذا كانت أوراق العمل محمية بكلمة مرور. |
| [Password](../../aspose.cells/protection/password/) { get; set; } | يمثل كلمة المرور لحماية ورقة العمل. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Copy](../../aspose.cells/protection/copy/)(Protection) | نسخ معلومات الحماية. |
| [GetPasswordHash](../../aspose.cells/protection/getpasswordhash/)() | يحصل على تجزئة كلمة المرور الحالية. |
| [VerifyPassword](../../aspose.cells/protection/verifypassword/)(string) | يتحقق من كلمة المرور. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ProtectionDemo
    {
        public static void ProtectionExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى إعدادات الحماية لورقة العمل
            Protection protection = worksheet.Protection;

            // تعيين خصائص الحماية المختلفة
            protection.AllowDeletingColumn = true;
            protection.AllowDeletingRow = true;
            protection.AllowFiltering = true;
            protection.AllowFormattingCell = true;
            protection.AllowFormattingColumn = true;
            protection.AllowFormattingRow = true;
            protection.AllowInsertingColumn = true;
            protection.AllowInsertingHyperlink = true;
            protection.AllowInsertingRow = true;
            protection.AllowSorting = true;
            protection.AllowUsingPivotTable = true;
            protection.AllowEditingContent = true;
            protection.AllowEditingObject = true;
            protection.AllowEditingScenario = true;
            protection.Password = "password123";
            protection.AllowSelectingLockedCell = true;
            protection.AllowSelectingUnlockedCell = true;

            // التحقق مما إذا كانت ورقة العمل محمية بكلمة مرور
            bool isProtectedWithPassword = protection.IsProtectedWithPassword;

            // حفظ المصنف
            workbook.Save("ProtectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


