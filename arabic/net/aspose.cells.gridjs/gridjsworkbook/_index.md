---
title: "الفئة GridJsWorkbook"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridJs.GridJsWorkbook. تمثل الفئة الرئيسية للدخول إلى GridJs"
type: docs
url: /ar/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

يمثل الفئة الرئيسية للدخول لـ GridJs

```csharp
public class GridJsWorkbook
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook/)() | ينشئ نسخة جديدة من GridJsWorkbook. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CacheDirectory](../../aspose.cells.gridjs/gridjsworkbook/cachedirectory/) { get; set; } | يحصل/يضبط دليل الذاكرة المؤقتة لتخزين ملف جدول البيانات. إذا لم يتم ضبطه، سنستخدم الخاصية الثابتة من [`FileCacheDirectory`](../config/filecachedirectory/) أو [`CacheImp`](./cacheimp/). |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings/) { get; set; } | يمثل إعدادات المصنف. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback/) { get; set; } | يحصل أو يضبط رد النداء التحذيري لاستيراد الملف. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [BurnRedactionFile](../../aspose.cells.gridjs/gridjsworkbook/burnredactionfile/)(string, string) | ينفذ (يطبق) جميع عمليات الإخفاء في دفتر العمل عن طريق إزالة أشكال الإخفاء وأشكال الهدف الخاصة بها أو مسح محتويات نطاق الخلايا المستهدف. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsworkbook/checkincacheforcollaborative/)(string) | تحقق مما إذا كانت نسخة المصنف موجودة في ذاكرة التخزين المؤقت. هذه الطريقة تُطبق فقط في وضع التعاون. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsworkbook/clearalljsoncache/)() | مسح جميع ذاكرة التخزين المؤقت لـ JSON |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsworkbook/clearjsoncacheforuid/)(string) | مسح ذاكرة التخزين المؤقت لـ JSON بناءً على uid (يُستخدم في سيناريوهات مثل UpdateCell التي لا تملك سوى uid). |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape/)(string, string) | ينسخ الصورة أو الشكل. |
| [Dispose](../../aspose.cells.gridjs/gridjsworkbook/dispose/)() | ينفّذ مهامًا معرفة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة تعيين الموارد غير المُدارة. |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson/)(string) | يحصل على سلسلة رسالة الخطأ بتنسيق JSON. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson)() | يحصل على سلسلة JSON من بيانات الذاكرة، اسم الملف الافتراضي في JSON هو: book1. |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson/#exporttojson_1)(string) | يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON. |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder/)(string, string) | يحصل على سلسلة JSON من بيانات الذاكرة، يحدد اسم ملف الإخراج في JSON. |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid/)(string, string) | يحصل على سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، ويحدد اسم ملف الإخراج في JSON. |
| [GetOle](../../aspose.cells.gridjs/gridjsworkbook/getole/)(string, string, int, out string) | يحصل على بيانات مصفوفة البايت للكائن OLE المضمن. |
| [GetSheetJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getsheetjsonwithcache/)(string, string, string) | احصل على JSON للورقة المحددة (مع التخزين المؤقت) |
| [GetWorkbookJsonWithCache](../../aspose.cells.gridjs/gridjsworkbook/getworkbookjsonwithcache/)(string, string) | الحصول على JSON كامل للدفتر (مع التخزين المؤقت) |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_3)(string) | يستورد ملف Excel من مسار الملف. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile)(Workbook) | يستورد ملف Excel من كائن Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_1)(Stream, GridLoadFormat) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_7)(string, string) | يستورد ملف Excel من مسار الملف. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_4)(string, Workbook) | يستورد ملف Excel من كائن Workbook. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_2)(Stream, GridLoadFormat, string) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_5)(string, Stream, GridLoadFormat) | يستورد ملف Excel من تدفق الملف. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_8)(string, string, string) | يستورد ملف Excel من مسار الملف وكلمة مرور الفتح. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile/#importexcelfile_6)(string, Stream, GridLoadFormat, string) | يستورد ملف Excel من تدفق الملف مع تنسيق التحميل وكلمة مرور الفتح. |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson/)(string) | يستورد ملف Excel من سلسلة بتنسيق JSON. |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage/)(string, string, Stream, string) | يدرج صورة في ورقة العمل من تدفق الملف أو URL (يجب توفير إما تدفق الملف أو URL) أو يدرج شكلًا عندما يكون p.type أحد AutoShapeType |
| [JsonToStream](../../aspose.cells.gridjs/gridjsworkbook/jsontostream/)(Stream, string, string) | إنشاء JSON من Workbook الموجود في الذاكرة وكتابته إلى الدفق المحدد. يمكن تخزين JSON الناتج مؤقتًا للحصول على استرجاع أسرع لاحقًا. الفروقات الرئيسية عن JsonToStreamByUid: - يستخدم هذا الأسلوب حالة Workbook الحالية في الذاكرة (حقل wb) - يقوم JsonToStreamByUid بإعادة تحميل Workbook من ملفات ذاكرة التخزين المؤقت .cells على القرص - استخدم هذا الأسلوب عندما تريد تصدير حالة دفتر العمل الحالية بعد التعديلات - استخدم JsonToStreamByUid عندما تحتاج إلى إعادة إنشاء JSON من حالة ملف مخزن مؤقتًا مسبقًا سلوك التخزين المؤقت (عند توفير uid): - يتحقق من ذاكرة التخزين المؤقت لـ JSON قبل الإنشاء (L1 الذاكرة + L2 القرص) - إذا فشل العثور في الذاكرة، ينشئ JSON من Workbook الموجود في الذاكرة - يخزن JSON المُنشأ في الذاكرة المؤقتة للطلبات المستقبلية |
| [JsonToStreamByUid](../../aspose.cells.gridjs/gridjsworkbook/jsontostreambyuid/)(Stream, string, string) | استرجع سلسلة JSON للملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، واضبط اسم ملف الإخراج في JSON، واكتبها إلى الدفق. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingjson/)(string, string) | يحصل على سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد. |
| [LazyLoadingStream](../../aspose.cells.gridjs/gridjsworkbook/lazyloadingstream/)(Stream, string, string) | استرجع سلسلة JSON للورقة المحددة في الملف من الذاكرة المؤقتة باستخدام المعرف الفريد المحدد، واكتبها إلى الدفق. |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson/)(string, string) | يطبق تحديثًا دفعيًا على بيانات الذاكرة. |
| [RedactFile](../../aspose.cells.gridjs/gridjsworkbook/redactfile/)(string, string, string[]) | ينفذ حذفًا على ملف Excel بناءً على مصفوفة من عمليات JSON. |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename/)(string, string, string) | يحفظ بيانات الذاكرة إلى ملف الذاكرة المؤقتة بالاسم المحدد ويضبط أيضًا كلمة مرور الفتح، تنسيق الحفظ يعتمد على امتداد اسم الملف. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile)(Stream) | يحفظ بيانات الذاكرة إلى الدفق، بناءً على تنسيق الملف الأصلي. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile/#savetoexcelfile_1)(string) | يحفظ بيانات الذاكرة إلى مسار الملف، إذا كان للملف امتداد، يكون تنسيق الحفظ بناءً على امتداد الملف. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml)(Stream) | يحفظ بيانات الذاكرة إلى الدفق، تنسيق الحفظ هو html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml/#savetohtml_1)(string) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو html. |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf)(Stream) | يحفظ بيانات الذاكرة إلى الدفق، تنسيق الحفظ هو pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf/#savetopdf_1)(string) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx)(Stream) | يحفظ بيانات الذاكرة إلى الدفق، تنسيق الحفظ هو xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx/#savetoxlsx_1)(string) | يحفظ بيانات الذاكرة إلى مسار الملف، تنسيق الحفظ هو xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload/)(GridInterruptMonitor, int) | يضبط InterruptMonitor لعملية التحميل. |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave/)(GridInterruptMonitor) | يضبط InterruptMonitor لعملية الحفظ. |
| [SetTransParentView](../../aspose.cells.gridjs/gridjsworkbook/settransparentview/)(string, string, bool) | يضبط شفافية أشكال الحذف في دفتر العمل. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsworkbook/translatesheetasync/)(string, string, ITextTranslator, string) | ترجمة جميع قيم السلاسل إلى اللغة المستهدفة في ورقة العمل. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell/)(string, string) | يطبق عملية التحديث. |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat/)(string) | يحصل على تنسيق التحميل بناءً على امتداد الملف |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream/)(string, string, string) | احصل على تدفق الصورة. |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl/)(string, string, string) | يحصل على عنوان URL للصورة. |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile/)(string) | ينشئ معرفًا فريدًا جديدًا لذاكرة التخزين المؤقت للملف باستخدام اسم الملف المعطى. |
| static [SetImageUrlBase](../../aspose.cells.gridjs/gridjsworkbook/setimageurlbase/)(string) | حدد عنوان URL لإجراء الحصول على الصورة الأساسية من المتحكم. |

## الحقول

| الاسم | الوصف |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp/) | تنفيذ مخصص لتخزين الذاكرة المؤقتة، إذا كنت ترغب في تخزين الذاكرة المؤقتة بطريقة التدفق، تحتاج إلى ضبطه وتنفيذه. |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine/) | تنفيذ مخصص لمحرك الحساب، إذا كنت ترغب في إجراء حساب مخصص، تحتاج إلى ضبطه وتنفيذه. |
| const [pictureType](../../aspose.cells.gridjs/gridjsworkbook/picturetype/) | قيمة ثابتة لنوع الصورة |
| static [UpdateMonitor](../../aspose.cells.gridjs/gridjsworkbook/updatemonitor/) | يحصل/يضبط مراقب التحديث لتتبع عملية التحديث |

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


