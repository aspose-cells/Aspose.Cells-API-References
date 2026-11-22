---
title: "تعداد GridRenameStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.GridDesktop.Data.GridRenameStrategy. خيار الاستراتيجية لأسماء الأعمدة المكررة"
type: docs
url: /ar/net/aspose.cells.griddesktop.data/gridrenamestrategy/
---
## GridRenameStrategy enumeration

خيار الاستراتيجية لأسماء الأعمدة المكررة.

```csharp
public enum GridRenameStrategy
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Exception | `0` | يرمي استثناءً. |
| Digit | `1` | مسمى بالرقم. ستصبح الأسماء المكررة ...1، ...2، إلخ. |
| Letter | `2` | مسمى بالحرف.. ستصبح الأسماء المكررة ...A، ...B، إلخ. |

### ملاحظات

عند معالجة البيانات مع رؤوس الأعمدة، تتطلب بعض السيناريوهات عدم تكرار الرؤوس لجميع الأعمدة. على سبيل المثال، عند تصدير البيانات إلى جدول بيانات ويتطلب أن يُؤخذ الرأس كاسم عمود جدول البيانات، تكون قيم الرؤوس المكررة غير صالحة. في مثل هذه الحالات، يمكن للمستخدم تحديد كيفية التعامل معها عن طريق تحديد هذه الإستراتيجية.

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


