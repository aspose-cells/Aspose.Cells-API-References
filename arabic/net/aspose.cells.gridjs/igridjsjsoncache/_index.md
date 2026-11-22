---
title: "الواجهة IGridJsJsonCache"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.GridJs.IGridJsJsonCache. واجهة تخزين مؤقت JSON يطبق العملاء استراتيجيات تخزين وإبطال محددة"
type: docs
url: /ar/net/aspose.cells.gridjs/igridjsjsoncache/
---
## IGridJsJsonCache interface

واجهة تخزين JSON المؤقت - يقوم العملاء بتنفيذ استراتيجيات التخزين والإبطال المحددة.

```csharp
public interface IGridJsJsonCache
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ClearAll](../../aspose.cells.gridjs/igridjsjsoncache/clearall/)() | مسح جميع التخزينات المؤقتة |
| [GetCacheKey](../../aspose.cells.gridjs/igridjsjsoncache/getcachekey/)(string, string) | إنشاء مفتاح تخزين مؤقت. يمكن للعملاء اتخاذ قرار تضمين معرف uid بناءً على متطلبات العمل. - إذا كان اسم الملف فقط هو المهم: تجاهل uid واستخدام fileName فقط (مستحسن، يسمح بمشاركة التخزين المؤقت عبر نفس الملف). - إذا كان التمييز بين الملفات ذات الاسم نفسه مطلوبًا: استخدم uid (وضع صارم). |
| [Invalidate](../../aspose.cells.gridjs/igridjsjsoncache/invalidate/)(string) | إبطال الإدخال المحدد في التخزين المؤقت. |
| [InvalidateAllForUid](../../aspose.cells.gridjs/igridjsjsoncache/invalidateallforuid/)(string) | إبطال جميع إدخالات التخزين المؤقت التي تحتوي على uid المحدد. هذا مفيد عندما لا تعرف اسم الملف الدقيق المستخدم في التخزين المؤقت. |
| [SetJson](../../aspose.cells.gridjs/igridjsjsoncache/setjson/)(string, string) | كتابة JSON في التخزين المؤقت. |
| [TryGetJson](../../aspose.cells.gridjs/igridjsjsoncache/trygetjson/)(string) | محاولة استرجاع JSON من التخزين المؤقت. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


