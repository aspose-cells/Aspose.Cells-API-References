---
title: "فئة GridJsService"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridJs.GridJsService. توفر واجهات برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم"
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

يوفر واجهات برمجة التطبيقات الأساسية للعمليات المستخدمة في إجراءات المتحكم.

```csharp
public class GridJsService : IGridJsService
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | المُنشئ لفئة GridJsService للمضيفين الذين يبنون كائن الخيارات بأنفسهم (مضيف المتصفح WASM وأي إعداد خادم غير DI). |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | المُنشئ الافتراضي لفئة GridJsService |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | يمثل إعدادات المصنف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | يطبق عملية إضافة صورة من ملف محلي (تأتي بايتات الملف من JS FormData أو أي مضيف). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | يطبق عملية إضافة صورة من ملف محلي. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | يطبق عملية إضافة صورة من عنوان URL بعيد. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | تحقق مما إذا كانت نسخة المصنف موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق فقط في وضع التعاون. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | يمسح جميع إدخالات ذاكرة التخزين المؤقت JSON (الذاكرة والقرص). |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | يمسح جميع إدخالات ذاكرة التخزين المؤقت JSON التي تخص المعرف الفريد المحدد. استدعِ هذا بعد تعديل ملف المصدر خارج النطاق حتى يُعيد الطلب التالي توليد JSON. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | يطبق عملية نسخ الصورة. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | هذه الطريقة مخصصة لجافا فقط، تُنفّذ طريقة destroy في DisposableBean، والتي سيتم استدعاؤها تلقائيًا بواسطة Spring عند انتهاء الطلب، في الواقع ستستدعي طريقة Dispose. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | يحصل على سلسلة JSON للملف وفقًا للمعرف الفريد المحدد. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | يحصل على سلسلة JSON للمصنف وفقًا للمعرف الفريد المحدد. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | اكتب سلسلة JSON للملف إلى التدفق. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | اكتب سلسلة JSON للمصنف إلى التدفق |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | اكتب سلسلة JSON للملف إلى التدفق وفقًا للمعرف الفريد المحدد. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | اكتب سلسلة JSON للمصنف إلى التدفق وفقًا للمعرف الفريد المحدد. |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | يطبق عملية تنزيل الملف |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | احصل على تدفق الملف |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | يحصل على رد النداء التحذيري المخصص لاستيراد الملف. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | احصل على تدفق الصورة. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | يحصل على عنوان URL للصورة. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | يكتب سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد إلى التدفق. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويحدد اسم ملف الإخراج في JSON. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | يحصل على بيانات مصفوفة البايت للكائن OLE المضمن. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | يضبط رد النداء التحذيري المخصص لاستيراد الملف. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | ترجمة جميع قيم السلاسل إلى اللغة المستهدفة في ورقة العمل. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | يطبق عملية التحديث. |

### انظر أيضًا

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


