---
title: "الواجهة IGridJsService"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "واجهة Aspose.Cells.GridJs.IGridJsService. تمثل واجهة واجهات برمجة التطبيقات للعمليات الأساسية المستخدمة في إجراءات المتحكم."
type: docs
url: /ar/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

يمثل واجهة برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم.

```csharp
public interface IGridJsService : IDisposable
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | يطبق عملية إضافة صورة من ملف محلي، مع أخذ بايتات الصورة مباشرة. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | يطبق عملية إضافة صورة من ملف محلي، مع أخذ ملفات النموذج المرفوعة. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | يطبق عملية إضافة صورة من عنوان URL بعيد. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | تحقق مما إذا كانت نسخة المصنف موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق فقط في وضع التعاون. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | يمسح جميع إدخالات ذاكرة التخزين المؤقت JSON (الذاكرة والقرص). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | يمسح جميع إدخالات ذاكرة التخزين المؤقت JSON التي تخص المعرف الفريد المحدد. استدعِ هذا بعد تعديل ملف المصدر خارج النطاق حتى يُعيد الطلب التالي توليد JSON. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | يطبق عملية نسخ الصورة. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | يحصل على سلسلة JSON للملف وفقًا للمعرف الفريد المحدد. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | يحصل على سلسلة JSON للمصنف وفقًا للمعرف الفريد المحدد. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | اكتب سلسلة JSON للمصنف إلى التدفق |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | اكتب سلسلة JSON للمصنف إلى التدفق |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | اكتب سلسلة JSON للملف إلى التدفق وفقًا للمعرف الفريد المحدد. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | اكتب سلسلة JSON للمصنف إلى التدفق وفقًا للمعرف الفريد المحدد. |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | يطبق عملية تنزيل الملف |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | احصل على تدفق الملف |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | يحصل على رد النداء التحذيري المخصص لاستيراد الملف. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | احصل على تدفق الصورة. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | يحصل على عنوان URL للصورة. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | يكتب سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد إلى التدفق. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويحدد اسم ملف الإخراج في JSON. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | يحصل على بيانات مصفوفة البايت للكائن OLE المضمن. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | يضبط رد النداء التحذيري المخصص لاستيراد الملف. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | يطبق عملية التحديث. |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


