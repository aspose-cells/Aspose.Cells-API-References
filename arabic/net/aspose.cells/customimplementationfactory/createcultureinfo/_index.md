---
title: CreateCultureInfo
second_title: Aspose.Cells لمرجع .NET API
description: أنشئ معلومات ثقافية واحدة بالمعرف المحدد .
type: docs
weight: 20
url: /ar/net/aspose.cells/customimplementationfactory/createcultureinfo/
---
## CustomImplementationFactory.CreateCultureInfo method

أنشئ معلومات ثقافية واحدة بالمعرف المحدد .

```csharp
public virtual CultureInfo CreateCultureInfo(int lcid)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| lcid | Int32 |  |

### قيمة الإرجاع

مثيل CultureInfo.

### ملاحظات

هذا التنفيذ مفيد للحالات: 1. قد لا تكون بعض الثقافات مدعومة من قبل بيئة المستخدم وقد يتسبب إنشاء CultureInfo المطلوبة بمعرف معين في حدوث استثناء . لتجنب الاستثناء ، يجوز للمستخدم تجاوز هذه الطريقة لتوفير مثيل CultureInfo صالح لـ واحد غير مدعوم. 2. قد يرغب المستخدم في تحديد بعض الخصائص المخصصة لبعض الثقافات للحصول على النتيجة المتوقعة للتنسيق. قد يؤثر مثيل CultureInfo الذي تم إرجاعه على النتيجة المنسقة . إذا كانت خاطئة ، فقد يتم تجاوز بعض خصائص مثيل CultureInfo الذي تم إرجاعه بواسطة محرك التنسيق المدمج الخاص بنا وفقًا لمتطلبات التنسيق لسيناريوهات مختلفة . إذا كان هذا صحيحًا ، فلن نقوم بذلك قم بتغيير أي خصائص لها واستخدمها لتنسيق القيم مباشرة . لذلك ، إذا كان المستخدم لديه spe الخصائص المخصصة المعتمدة لمثيل CultureInfo الذي تم إرجاعه ، يرجى التأكد من صحة UseUserOverride الخاص به.

### أنظر أيضا

* class [CustomImplementationFactory](../../customimplementationfactory)
* مساحة الاسم [Aspose.Cells](../../customimplementationfactory)
* المجسم [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->