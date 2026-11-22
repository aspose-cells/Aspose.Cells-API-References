---
title: "GridJsWorkbook.JsonToStream"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GridJsWorkbook. تولد JSON من المصنف الموجود في الذاكرة وتكتبها إلى الدفق المحدد. يمكن اختيارياً تخزين JSON المُولد في الذاكرة المؤقتة للحصول على استرجاع أسرع لاحقاً. الفروقات الرئيسية عن JsonToStreamByUid: تستخدم هذه الطريقة حالة المصنف الحالية في الذاكرة (حقل wb). يقوم JsonToStreamByUid بإعادة تحميل المصنف من ملفات الذاكرة المؤقتة .cells على القرص. استخدم هذه الطريقة عندما تريد تصدير حالة المصنف الحالية بعد التعديلات. استخدم JsonToStreamByUid عندما تحتاج إلى إعادة توليد JSON من حالة ملف مخزن مسبقاً. سلوك التخزين المؤقت عندما يتم توفير uid: يتحقق من ذاكرة التخزين المؤقت لـ JSON قبل الإنشاء (الذاكرة L1، القرص L2). إذا فشل التخزين المؤقت، يولد JSON من المصنف في الذاكرة. يخزن JSON المُولد في الذاكرة المؤقتة للطلبات المستقبلية."
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsworkbook/jsontostream/
---
## GridJsWorkbook.JsonToStream method

إنشاء JSON من Workbook الموجود في الذاكرة وكتابته إلى الدفق المحدد. يمكن تخزين JSON الناتج مؤقتًا للحصول على استرجاع أسرع لاحقًا. الفروقات الرئيسية عن JsonToStreamByUid: - يستخدم هذا الأسلوب حالة Workbook الحالية في الذاكرة (حقل wb) - يقوم JsonToStreamByUid بإعادة تحميل Workbook من ملفات ذاكرة التخزين المؤقت .cells على القرص - استخدم هذا الأسلوب عندما تريد تصدير حالة دفتر العمل الحالية بعد التعديلات - استخدم JsonToStreamByUid عندما تحتاج إلى إعادة إنشاء JSON من حالة ملف مخزن مؤقتًا مسبقًا سلوك التخزين المؤقت (عند توفير uid): - يتحقق من ذاكرة التخزين المؤقت لـ JSON قبل الإنشاء (L1 الذاكرة + L2 القرص) - إذا فشل العثور في الذاكرة، ينشئ JSON من Workbook الموجود في الذاكرة - يخزن JSON المُنشأ في الذاكرة المؤقتة للطلبات المستقبلية

```csharp
public void JsonToStream(Stream stream, string filename, string uid = null)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| تدفق | Stream | دفق الإخراج لكتابة بيانات JSON إليه. |
| اسم الملف | String | يحدد اسم الملف في JSON. إذا تم تعيينه إلى null، يكون اسم الملف الافتراضي: book1. |
| uid | String | معرف فريد اختياري لتخزين JSON مؤقتاً. عند توفيره، يتيح البحث في الذاكرة المؤقتة والتخزين. |

### انظر أيضًا

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


