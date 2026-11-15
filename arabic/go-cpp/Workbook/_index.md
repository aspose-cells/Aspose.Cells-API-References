---
title: "فئة Workbook"
linktitle: "Workbook"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "فئة Workbook. يغلف الكائن الذي يمثل workbook في Go."
type: docs
weight: 200
url: /ar/go-cpp/workbook/
---

## Workbook class

يمثل كائن الجذر لإنشاء جدول بيانات Excel.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## المُنشئات

| طريقة | الوصف |
| --- | --- |
| [NewWorkbook](./newworkbook/) | ينشئ نسخة جديدة من فئة Workbook. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | ينشئ نسخة جديدة من فئة Workbook. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | ينشئ نسخة جديدة فارغة من فئة Workbook مع الخيارات |
| [NewWorkbook_String](./newworkbook_string/) | ينشئ نسخة جديدة من فئة Workbook ويفتح ملفًا. |
| [NewWorkbook_Stream](./newworkbook_stream/) | ينشئ نسخة جديدة من فئة Workbook ويفتح تدفقًا. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | ينشئ نسخة جديدة من فئة Workbook ويفتح ملفًا. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | ينشئ نسخة جديدة من فئة Workbook ويفتح التدفق. |

## طرق

| طريقة | الوصف |
| --- | --- |
| [IsNull](./isnull/) | يتحقق مما إذا كان كائن التنفيذ هو nullptr. |
| [GetSettings](./getsettings/) | يمثل إعدادات دفتر العمل. |
| [ParseFormulas](./parseformulas/) | يقوم بتحليل جميع الصيغ التي لم يتم تحليلها عندما تم تحميلها من ملف القالب أو تعيينها إلى خلية. |
| [StartAccessCache](./startaccesscache/) | يبدأ الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات. |
| [CloseAccessCache](./closeaccesscache/) | يغلق الجلسة التي تستخدم الذاكرات المؤقتة للوصول إلى البيانات. |
| [Save_String_SaveFormat](./save_string_saveformat/) | يحفظ دفتر العمل على القرص. |
| [Save_String](./save_string/) | احفظ دفتر العمل على القرص. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | يحفظ دفتر العمل على القرص. |
| [Save_SaveFormat](./save_saveformat/) | يحفظ دفتر العمل إلى الدفق. |
| [Save_SaveOptions](./save_saveoptions/) | يحفظ دفتر العمل إلى الدفق. |
| [SaveToStream](./savetostream/) | يحفظ ملف Excel إلى كائن MemoryStream كملف Excel97-2003 xls ويعيده. |
| [GetWorksheets](./getworksheets/) | يحصل على مجموعة WorksheetCollection في جدول البيانات. |
| [IsLicensed](./islicensed/) | يشير إلى ما إذا تم تعيين الترخيص. |
| [RemoveUnusedStyles](./removeunusedstyles/) | إزالة جميع الأنماط غير المستخدمة. |
| [CreateStyle](./createstyle/) | ينشئ نمطًا جديدًا. |
| [CreateStyle_Bool](./createstyle_bool/) | ينشئ نمطًا جديدًا. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | ينشئ نمطًا مدمجًا حسب النوع المحدد. |
| [CreateCellsColor](./createcellscolor/) | ينشئ كائن CellsColor. |
| [Replace_String_String](./replace_string_string/) | يستبدل قيمة الخلية بسلسلة جديدة. |
| [Replace_String_Int](./replace_string_int/) | يستبدل قيمة الخلية بعدد صحيح جديد. |
| [Replace_String_Double](./replace_string_double/) | يستبدل قيمة الخلية برقم مزدوج جديد. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | يستبدل قيمة الخلية بمصفوفة سلاسل جديدة. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | يستبدل قيم الخلايا بمصفوفة أعداد صحيحة. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | يستبدل قيم الخلايا بمصفوفة أعداد مزدوجة. |
| [Replace_Bool_Object](./replace_bool_object/) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace_Int_Object](./replace_int_object/) | يستبدل قيم الخلايا ببيانات جديدة. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | يستبدل قيمة الخلية بسلسلة جديدة. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | ينسخ كائن Workbook آخر. |
| [Copy_Workbook](./copy_workbook/) | ينسخ البيانات من كائن Workbook المصدر. |
| [Combine](./combine/) | يجمع كائن Workbook آخر. |
| [GetColors](./getcolors/) | يعيد الألوان في لوحة الألوان لجدول البيانات. |
| [GetStyleInPool](./getstyleinpool/) | يحصل على النمط في مجموعة الأنماط. سيتم جمع جميع الأنماط في دفتر العمل في مجموعة. هناك فهرس إشارة بسيط فقط في الخلايا. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | يحصل على عدد الأنماط في مجموعة الأنماط. |
| [GetFonts](./getfonts/) | يحصل على جميع الخطوط في مجموعة الأنماط. |
| [GetNamedStyle](./getnamedstyle/) | يحصل على النمط المسمى في مجموعة الأنماط. |
| [MergeNamedStyles](./mergenamedstyles/) | يدمج الأنماط المسماة من ملف Excel الآخر. |
| [ChangePalette](./changepalette/) | يغيّر لوحة الألوان للجدول في الفهرس المحدد. |
| [IsColorInPalette](./iscolorinpalette/) | يتحقق مما إذا كان اللون موجودًا في لوحة الألوان للجدول. |
| [CalculateFormula](./calculateformula/) | يحسب نتيجة الصيغ. |
| [CalculateFormula_Bool](./calculateformula_bool/) | يحسب نتيجة الصيغ. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | حساب الصيغ في هذا المصنف. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) لن يتم حساب الصيغ الأخرى في المصنف بشكل متكرر حتى لو تم استخدامها بواسطة صيغ المصفوفة الديناميكية. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | يقوم بتحديث صيغ المصفوفة الديناميكية (تنتشر إلى نطاق جديد من الخلايا المجاورة وفقًا للبيانات الحالية) |
| [GetDefaultStyle](./getdefaultstyle/) | يحصل أو يعيّن كائن النمط الافتراضي للمصنف. |
| [SetDefaultStyle](./setdefaultstyle/) | يحصل أو يعيّن كائن النمط الافتراضي للمصنف. |
| [GetMatchingColor](./getmatchingcolor/) | ابحث عن اللون الأنسب في لوحة الألوان الحالية. |
| [IsDigitallySigned](./isdigitallysigned/) | يشير إلى ما إذا كان هذا الجدول موقعًا رقمياً. |
| [SetEncryptionOptions](./setencryptionoptions/) | تعيين خيارات التشفير. |
| [Protect](./protect/) | يحمي مصنفًا. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | يحمي مصنفًا مشتركًا. |
| [Unprotect](./unprotect/) | يفك حماية مصنف. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | يفك حماية مصنف مشترك. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | يشير إلى ما إذا كان الهيكل أو النافذة محميًا بكلمة مرور. |
| [RemoveMacro](./removemacro/) | يزيل VBA/ماكرو من هذا الجدول. |
| [GetVbaProject](./getvbaproject/) | يحصل على VbaProject في جدول. |
| [RemoveDigitalSignature](./removedigitalsignature/) | يزيل التوقيع الرقمي من هذا الجدول. |
| [AcceptAllRevisions](./acceptallrevisions/) | يقبل جميع التغييرات المتتبعة في المصنف. |
| [GetHasMacro](./gethasmacro/) | يشير إلى ما إذا كان هذا الجدول يحتوي على ماكرو/VBA. |
| [GetHasRevisions](./gethasrevisions/) | يحصل على ما إذا كان المصنف يحتوي على أي تغييرات متتبعة |
| [GetFileName](./getfilename/) | يحصل ويعيّن اسم الملف الحالي. |
| [SetFileName](./setfilename/) | يحصل ويعيّن اسم الملف الحالي. |
| [GetDataSorter](./getdatasorter/) | يحصل على كائن DataSorter لفرز البيانات. |
| [GetThemeColor](./getthemecolor/) | يحصل على لون السمة. |
| [SetThemeColor](./setthemecolor/) | يضبط لون السمة |
| [GetTheme](./gettheme/) | يحصل على اسم السمة. |
| [CustomTheme](./customtheme/) | يخصص السمة. |
| [CopyTheme](./copytheme/) | ينسخ السمة من دفتر عمل آخر. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | يحدّث تعريف الدوال المخصصة. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | إذا كان دفتر العمل هذا يحتوي على روابط خارجية إلى مصدر بيانات آخر،Aspose.Cells سيحاول استرجاع أحدث البيانات من المصادر المعطاة. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | يعيد مجموعة DocumentProperty تمثل جميع خصائص المستند المدمجة في جدول البيانات. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | يعيد مجموعة DocumentProperty تمثل جميع خصائص المستند المخصصة في جدول البيانات. |
| [GetFileFormat](./getfileformat/) | يحصل على ويضبط تنسيق الملف. |
| [SetFileFormat](./setfileformat/) | يحصل على ويضبط تنسيق الملف. |
| [GetHasCustomFunction](./gethascustomfunction/) | يكشف ما إذا كان هناك دالة مخصصة مستخدمة في دفتر العمل هذا، مثل في صيغة الخلية، أو في الأسماء المعرفة... |
| [GetInterruptMonitor](./getinterruptmonitor/) | يحصل على أو يضبط مراقب المقاطعة. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | يحصل على أو يضبط مراقب المقاطعة. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | يضبط مراقب المقاطعة. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | يحصل على قائمة كائنات ContentTypeProperty في دفتر العمل. |
| [GetCustomXmlParts](./getcustomxmlparts/) | يمثل جزء تخزين بيانات XML مخصص (بيانات XML مخصصة داخل حزمة). |
| [GetDataMashup](./getdatamashup/) | يحصل على بيانات الدمج. |
| [GetRibbonXml](./getribbonxml/) | يحصل على ويضبط ملف XML الذي يعرّف واجهة الشريط. |
| [SetRibbonXml](./setribbonxml/) | يحصل على ويضبط ملف XML الذي يعرّف واجهة الشريط. |
| [GetAbsolutePath](./getabsolutepath/) | يحصل على ويضبط المسار المطلق للملف. |
| [SetAbsolutePath](./setabsolutepath/) | يحصل على ويضبط المسار المطلق للملف. |
| [GetDataConnections](./getdataconnections/) | يحصل على مجموعة ExternalConnection. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | يستورد/يحدّث ملف بيانات XML إلى دفتر العمل. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | يستورد/يحدّث ملف بيانات XML إلى دفتر العمل. |
| [ExportXml_String_String](./exportxml_string_string/) | يصدّر بيانات XML المرتبطة بخريطة XML المحددة. |
| [ExportXml_String](./exportxml_string/) | يصدّر بيانات XML. |
| [SetDigitalSignature](./setdigitalsignature/) | يضبط التوقيع الرقمي لملف جدول بيانات (Excel2007 وما بعده). |
| [AddDigitalSignature](./adddigitalsignature/) | يضيف التوقيع الرقمي إلى ملف جدول بيانات OOXML (Excel2007 وما بعده). |
| [GetDigitalSignature](./getdigitalsignature/) | يحصل على التوقيع الرقمي من الملف. |
| [RemovePersonalInformation](./removepersonalinformation/) | يزيل المعلومات الشخصية. |
| [GetDataModel](./getdatamodel/) | يحصل على نموذج البيانات في دفتر العمل. |
| [RefreshAll](./refreshall/) | تحديث الأشكال المرتبطة، جميع جداول Pivot والرسوم البيانية بمصدر Pivot. |
| [Dispose](./dispose/) | يؤدي مهامًا محددة من قبل التطبيق مرتبطة بتحرير أو إطلاق أو إعادة ضبط الموارد غير المُدارة. |
