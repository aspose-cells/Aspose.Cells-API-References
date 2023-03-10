---
title: PdfSaveOptions الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1180
url: /ar/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions الدرجة
يمثل خيارات حفظ ملف pdf.



**ميراث:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/ar/python-net/aspose.cells/saveoptions)



يكشف نوع PdfSaveOptions الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [PdfSaveOptions()](/cells/ar/python-net/aspose.cells/pdfsaveoptions/__init__/#) | ينشئ خيارات لحفظ ملف pdf.|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [save_format](/cells/ar/python-net/aspose.cells/pdfsaveoptions/save_format) | يحصل على تنسيق ملف الحفظ.|
| [clear_data](/cells/ar/python-net/aspose.cells/pdfsaveoptions/clear_data) | اجعل المصنف فارغًا بعد حفظ الملف.|
| [cached_file_folder](/cells/ar/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | يتم استخدام مجلد الملف المخزن مؤقتًا لتخزين بعض البيانات الكبيرة.|
| [validate_merged_areas](/cells/ar/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | يشير إلى ما إذا كان يجب التحقق من صحة الخلايا المدمجة قبل حفظ الملف.|
| [merge_areas](/cells/ar/python-net/aspose.cells/pdfsaveoptions/merge_areas) | يشير إلى ما إذا كان يتم دمج مناطق التنسيق الشرطي والتحقق من الصحة قبل حفظ الملف.|
| [create_directory](/cells/ar/python-net/aspose.cells/pdfsaveoptions/create_directory) | إذا كان صحيحًا وكان الدليل غير موجود ، فسيتم إنشاء الدليل تلقائيًا قبل حفظ الملف.|
| [sort_names](/cells/ar/python-net/aspose.cells/pdfsaveoptions/sort_names) | يشير إلى ما إذا كان يتم فرز الأسماء المعرفة قبل حفظ الملف.|
| [sort_external_names](/cells/ar/python-net/aspose.cells/pdfsaveoptions/sort_external_names) |يشير إلى ما إذا كان يتم فرز الأسماء المعرفة الخارجية قبل حفظ الملف.|
| [refresh_chart_cache](/cells/ar/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) | يشير إلى ما إذا كان يتم تحديث بيانات ذاكرة التخزين المؤقت للرسم البياني أم لا|
| [warning_callback](/cells/ar/python-net/aspose.cells/pdfsaveoptions/warning_callback) | يحصل أو يحدد رد الاتصال التحذيري.|
| [update_smart_art](/cells/ar/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | يشير إلى ما إذا كان يتم تحديث إعداد الفن الذكي.<br/> القيمة الافتراضية هي كاذبة.|
| [default_font](/cells/ar/python-net/aspose.cells/pdfsaveoptions/default_font) | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ،<br/>قد تظهر على شكل كتلة في صورة pdf.<br/>قم بتعيين الخط الافتراضي مثل MingLiu أو MS Gothic لإظهار هذه الأحرف.<br/> إذا لم يتم تعيين هذه الخاصية ، فسيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار أحرف unicode هذه.|
| [check_workbook_default_font](/cells/ar/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ،<br/>قد تظهر على شكل كتلة في صورة pdf.<br/> اضبط هذا على صواب لمحاولة استخدام الخط الافتراضي للمصنف لإظهار هذه الأحرف أولاً.|
| [check_font_compatibility](/cells/ar/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) |يشير إلى ما إذا كان سيتم التحقق من توافق الخط لكل حرف في النص.|
| [is_font_substitution_char_granularity](/cells/ar/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | الإشارة إلى ما إذا كان سيتم استبدال خط الحرف فقط عندما لا يكون خط الخلية متوافقًا معه.|
| [one_page_per_sheet](/cells/ar/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | إذا كانت OnePagePerSheet صحيحة ، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط نتيجة لذلك.<br/> سيكون حجم الورق الخاص بإعداد الصفحات غير صالح ، والإعدادات الأخرى لإعداد الصفحات<br/> ستظل نافذة المفعول.|
| [all_columns_in_one_page_per_sheet](/cells/ar/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | إذا كانت AllColumnsInOnePagePerSheet صحيحة ، فسيتم إخراج محتوى العمود بالكامل في ورقة واحدة إلى صفحة واحدة فقط في النتيجة.<br/> سيتم تجاهل عرض حجم الورق الخاص بإعداد الصفحات والإعدادات الأخرى لإعداد الصفحات<br/> ستظل نافذة المفعول.|
| [ignore_error](/cells/ar/python-net/aspose.cells/pdfsaveoptions/ignore_error) | يشير إلى ما إذا كنت بحاجة إلى إخفاء الخطأ أثناء العرض.<br/> يمكن أن يكون الخطأ خطأ في الشكل ، الصورة ، عرض المخطط ، إلخ.|
| [output_blank_page_when_nothing_to_print](/cells/ar/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | يشير إلى ما إذا كان سيتم إخراج صفحة فارغة في حالة عدم وجود شيء للطباعة.|
| [page_index](/cells/ar/python-net/aspose.cells/pdfsaveoptions/page_index) | الحصول على أو تحديد الفهرس الذي يستند إلى 0 للصفحة الأولى لحفظها.|
| [page_count](/cells/ar/python-net/aspose.cells/pdfsaveoptions/page_count) | الحصول على أو تحديد عدد الصفحات المراد حفظها.|
| [printing_page_type](/cells/ar/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | يشير إلى الصفحات التي لن تتم طباعتها.|
| [gridline_type](/cells/ar/python-net/aspose.cells/pdfsaveoptions/gridline_type) | الحصول على نوع خط الشبكة أو تعيينه.|
| [text_cross_type](/cells/ar/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | الحصول على عرض نوع النص أو تعيينه عندما يكون عرض النص أكبر من عرض الخلية.|
| [default_edit_language](/cells/ar/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | الحصول على أو تعيين لغة التحرير الافتراضية.|
| [sheet_set](/cells/ar/python-net/aspose.cells/pdfsaveoptions/sheet_set) |الحصول على الأوراق أو تعيينها للعرض. الافتراضي هو كل الأوراق المرئية في المصنف: [SheetSet.visible](/cells/ar/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/ar/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | تنفذ هذه الواجهة للحصول على DrawObject و Bound عند العرض.|
| [page_saving_callback](/cells/ar/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) | التحكم / الإشارة إلى التقدم المحرز في عملية حفظ الصفحة.|
| [embed_standard_windows_fonts](/cells/ar/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | صحيح لدمج خطوط الكتابة الحقيقية.<br/>يؤثر فقط على أحرف ASCII من 32 إلى 127.<br/>يتم دائمًا تضمين خطوط رموز الأحرف الأكبر من 127.<br/>يتم دائمًا تضمين الخطوط للمعيار PDF / A-1a ، PDF / A-1b.<br/> الافتراضي هو الصحيح.|
| [bookmark](/cells/ar/python-net/aspose.cells/pdfsaveoptions/bookmark) |الحصول على العنصر [PdfBookmarkEntry](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry) وتعيينه.|
| [compliance](/cells/ar/python-net/aspose.cells/pdfsaveoptions/compliance) | سيتم تحويل المصنف إلى pdf وفقًا لـ PdfCompliance في هذه الخاصية.|
| [security_options](/cells/ar/python-net/aspose.cells/pdfsaveoptions/security_options) | عيّن هذه الخيارات ، عندما يكون الأمان مطلوبًا في نتيجة xls2pdf.|
| [image_type](/cells/ar/python-net/aspose.cells/pdfsaveoptions/image_type) | يمثل نوع الصورة عند تحويل الرسم البياني والشكل.|
| [calculate_formula](/cells/ar/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | يشير إلى ما إذا كان سيتم حساب الصيغ قبل حفظ ملف pdf.|
| [pdf_compression](/cells/ar/python-net/aspose.cells/pdfsaveoptions/pdf_compression) | أشر إلى خوارزمية الضغط|
| [created_time](/cells/ar/python-net/aspose.cells/pdfsaveoptions/created_time) | الحصول على وتعيين وقت إنشاء مستند pdf.|
| [producer](/cells/ar/python-net/aspose.cells/pdfsaveoptions/producer) | الحصول على وتعيين منتج مستند pdf الذي تم إنشاؤه.|
| [optimization_type](/cells/ar/python-net/aspose.cells/pdfsaveoptions/optimization_type) | يحصل على نوع تحسين pdf ويعينه.|
| [custom_properties_export](/cells/ar/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | الحصول على أو تحديد قيمة تحدد طريقة تصدير [CustomDocumentPropertyCollection](/cells/ar/python-net/aspose.cells.properties/customdocumentpropertycollection) إلى ملف PDF. القيمة الافتراضية هي بلا.|
| [export_document_structure](/cells/ar/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | يشير إلى ما إذا كان سيتم تصدير بنية المستند.|
| [emf_render_setting](/cells/ar/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | الإعداد لعرض ملف تعريف Emf.|
| [display_doc_title](/cells/ar/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | يشير إلى ما إذا كان يجب أن يعرض شريط عنوان النافذة عنوان المستند.|
| [font_encoding](/cells/ar/python-net/aspose.cells/pdfsaveoptions/font_encoding) | الحصول على أو تعيين ترميز الخطوط المضمنة في ملف pdf.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/ar/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | يضبط PPI المطلوب (بكسل لكل بوصة) لإعادة تشكيل الصور وجودة jpeg.<br/> سيتم تحويل جميع الصور إلى JPEG بإعداد الجودة المحدد ،<br/>والصور التي تكون أكبر من PPI المحدد (بكسل لكل بوصة) سيتم إعادة تشكيلها.|



###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [CustomDocumentPropertyCollection](/cells/ar/python-net/aspose.cells.properties/customdocumentpropertycollection)
* فئة [PaginatedSaveOptions](/cells/ar/python-net/aspose.cells/paginatedsaveoptions)
* فئة [PdfBookmarkEntry](/cells/ar/python-net/aspose.cells.rendering/pdfbookmarkentry)
* فئة [PdfSaveOptions](/cells/ar/python-net/aspose.cells/pdfsaveoptions)
* فئة [SaveOptions](/cells/ar/python-net/aspose.cells/saveoptions)
