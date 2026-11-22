---
title: "IGridJsJsonCache.GetCacheKey"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة IGridJsJsonCache. إنشاء مفتاح للذاكرة المؤقتة. يمكن للعملاء اتخاذ قرار تضمين uid بناءً على متطلبات العمل. إذا كان اسم الملف فقط هو المهم، تجاهل uid واستخدم fileName فقط؛ يُنصح بذلك لتسمح بمشاركة الذاكرة المؤقتة عبر نفس الملف. إذا كان من الضروري تمييز الملفات التي لها نفس الاسم، استخدم وضع uid الصارم"
type: docs
url: /ar/net/aspose.cells.gridjs/igridjsjsoncache/getcachekey/
---
## IGridJsJsonCache.GetCacheKey method

إنشاء مفتاح تخزين مؤقت. يمكن للعملاء اتخاذ قرار تضمين معرف uid بناءً على متطلبات العمل. - إذا كان اسم الملف فقط هو المهم: تجاهل uid واستخدام fileName فقط (مستحسن، يسمح بمشاركة التخزين المؤقت عبر نفس الملف). - إذا كان التمييز بين الملفات ذات الاسم نفسه مطلوبًا: استخدم uid (وضع صارم).

```csharp
public string GetCacheKey(string uid, string fileName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| uid | String | معرف فريد للملف (قد يختلف مع كل تحميل) |
| fileName | String | اسم الملف الأصلي |

### قيمة الإرجاع

مفتاح الذاكرة المؤقتة

### انظر أيضًا

* interface [IGridJsJsonCache](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


