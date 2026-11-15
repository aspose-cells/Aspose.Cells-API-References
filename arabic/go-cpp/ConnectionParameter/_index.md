---
title: "ConnectionParameter فئة"
linktitle: "ConnectionParameter"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "ConnectionParameter فئة. يغلف الكائن الذي يمثل connectionparameter في Go."
type: docs
weight: 200
url: /ar/go-cpp/connectionparameter/
---

## ConnectionParameter class

يحدد الخصائص المتعلقة بأي معلمات تُستخدم مع اتصالات البيانات الخارجية. المعلمات صالحة لـ ODBC واستعلامات الويب.

```go

type ConnectionParameter struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSqlType](./getsqltype/) | نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC. |
| [SetSqlType](./setsqltype/) | نوع بيانات SQL للمعامل. صالح فقط لمصادر ODBC. |
| [GetRefreshOnChange](./getrefreshonchange/) | علامة تشير إلى ما إذا كان يجب أن يتم تحديث الاستعلام تلقائيًا عندما يتغير محتوى acell الذي يوفر قيمة المعامل. إذا كان true، يتم تحديث البيانات الخارجية refreshedusing قيمة المعامل الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية datais فقط عندما يطلبها المستخدم، أو عندما يؤدي حدث آخر إلى التحديث (مثال، فتح المصنف). |
| [SetRefreshOnChange](./setrefreshonchange/) | علامة تشير إلى ما إذا كان يجب أن يتم تحديث الاستعلام تلقائيًا عندما يتغير محتوى acell الذي يوفر قيمة المعامل. إذا كان true، يتم تحديث البيانات الخارجية refreshedusing قيمة المعامل الجديدة في كل مرة يحدث فيها تغيير. إذا كان false، يتم تحديث البيانات الخارجية datais فقط عندما يطلبها المستخدم، أو عندما يؤدي حدث آخر إلى التحديث (مثال، فتح المصنف). |
| [GetPrompt](./getprompt/) | سلسلة مطالبة للمعامل. تُعرض على مستخدم الجدول مع واجهة إدخال UIto لجمع قيمة المعامل قبل تحديث البيانات الخارجية. تُستخدم فقط عندما whenparameterType = prompt. |
| [SetPrompt](./setprompt/) | سلسلة مطالبة للمعامل. تُعرض على مستخدم الجدول مع واجهة إدخال UIto لجمع قيمة المعامل قبل تحديث البيانات الخارجية. تُستخدم فقط عندما whenparameterType = prompt. |
| [GetType](./gettype/) | نوع المعامل المستخدم. إذا كان parameterType=value، فستُستخدم القيمة من boolean أو double أو integer أو string. في هذه الحالة، من المتوقع أن يتم تحديد واحد فقط من {boolean, double, integer, or string}. |
| [SetType](./settype/) | نوع المعامل المستخدم. إذا كان parameterType=value، فستُستخدم القيمة من boolean أو double أو integer أو string. في هذه الحالة، من المتوقع أن يتم تحديد واحد فقط من {boolean, double, integer, or string}. |
| [GetName](./getname/) | اسم المعامل. |
| [SetName](./setname/) | اسم المعامل. |
| [GetCellReference](./getcellreference/) | مرجع الخلية الذي يشير إلى أي قيمة خلية تُستخدم لمعلمة الاستعلام. تُستخدم فقط عندما يكون parameterType هو cell. |
| [SetCellReference](./setcellreference/) | مرجع الخلية الذي يشير إلى أي قيمة خلية تُستخدم لمعلمة الاستعلام. تُستخدم فقط عندما يكون parameterType هو cell. |
| [GetValue](./getvalue/) | قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية valueto تُستخدم كمعلمة استعلام. تُستخدم فقط عندما يكون parameterType هو value. |
| [SetValue](./setvalue/) | قيمة عددية غير صحيحة، قيمة صحيحة، قيمة نصية أو قيمة منطقية valueto تُستخدم كمعلمة استعلام. تُستخدم فقط عندما يكون parameterType هو value. |
