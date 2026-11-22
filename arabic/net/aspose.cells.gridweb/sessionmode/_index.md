---
title: "تعداد SessionMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.GridWeb.SessionMode. يمثل وضع الجلسة للشبكة."
type: docs
url: /ar/net/aspose.cells.gridweb/sessionmode/
---
## SessionMode enumeration

يمثل وضع الجلسة للشبكة.

```csharp
public enum SessionMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Session | `0` | يستخدم جلسة النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا. |
| ViewState | `1` | يستخدم ViewState الصفحة لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا. |
| Custom | `2` | يستخدم حدث LoadCustomData لتحميل بيانات ورقة الشبكة يدويًا. ويستخدم حدث SheetDataUpdated لحفظ بيانات ورقة الشبكة. |
| File | `3` | يستخدم ملف النظام لتخزين/استعادة بيانات ورقة الشبكة تلقائيًا، يحتاج المستخدم إلى ضبط SessionStorePath لتحديد دليل الملف. |

### انظر أيضًا

* namespace [Aspose.Cells.GridWeb](../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../)


