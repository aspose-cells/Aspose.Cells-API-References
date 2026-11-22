---
title: "MainWeb.OnSubmitClientFunction"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MainWeb. تحصل أو تعيين الدالة العميلة التي تُستدعى قبل إرسال التحكم من جانب العميل. يجب إعلان الدالة العميلة هكذا function MyOnSubmitarg cancelEdit  return true المتغير arg هو معامل الإرسال الذي يحتوي على الأمر لإرساله إلى الخادم. المتغير cancelEdit هو قيمة منطقية تشير إلى ما إذا كان التحكم قد تجاهل إدخال المستخدم قبل الإرسال. سيستمر التحكم في الإرسال إذا أعادت الدالة true. ملاحظة يمكنك استخدام المؤشر this في الدالة العميلة للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث"
type: docs
url: /ar/net/aspose.cells.gridweb/mainweb/onsubmitclientfunction/
---
## MainWeb.OnSubmitClientFunction property

الحصول أو تعيين الدالة الجانبية للعميل التي سيتم استدعاؤها قبل إرسال التحكم من جانب العميل. يجب إعلان دالة العميل كما يلي: function MyOnSubmit(arg, cancelEdit) { return true;} المتغيّر arg هو معطى الإرسال، يحتوي على الأمر الذي يُرسل إلى الخادم. المتغيّر cancelEdit هو قيمة منطقية تشير إلى ما إذا كان التحكم قد تجاهل إدخال المستخدم قبل الإرسال. سيستمر التحكم في الإرسال إذا أعادت الدالة true. ملاحظة: يمكنك استخدام المؤشر "this" في دالة العميل للإشارة إلى عنصر التحكم الشبكي الذي يطلق الحدث.

```csharp
public string OnSubmitClientFunction { get; set; }
```

### انظر أيضًا

* class [MainWeb](../)
* namespace [Aspose.Cells.GridWeb](../../../aspose.cells.gridweb/)
* assembly [Aspose.Cells.GridWeb](../../../)


