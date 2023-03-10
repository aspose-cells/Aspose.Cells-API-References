---
title: HtmlLoadOptions الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 770
url: /ar/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  HtmlLoadOptions الدرجة
يمثل خيارات عند استيراد ملف html.



**ميراث:** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions)



يكشف نوع HtmlLoadOptions الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [HtmlLoadOptions()](/cells/ar/python-net/aspose.cells/htmlloadoptions/__init__/#) | ينشئ خيارات لتحميل الملف.|
| [HtmlLoadOptions(load_format)](/cells/ar/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) | ينشئ خيارات لتحميل الملف.|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [load_format](/cells/ar/python-net/aspose.cells/htmlloadoptions/load_format) | يحصل على تنسيق التحميل.|
| [password](/cells/ar/python-net/aspose.cells/htmlloadoptions/password) | الحصول على كلمة المرور الخاصة بالمصنف وتعيينها.|
| [parsing_formula_on_open](/cells/ar/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) | يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف.|
| [parsing_pivot_cached_records](/cells/ar/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) | يشير إلى ما إذا كان تحليل السجلات المحورية المخزنة مؤقتًا عند تحميل الملف.<br/> القيمة الافتراضية هي كاذبة.|
| [language_code](/cells/ar/python-net/aspose.cells/htmlloadoptions/language_code) | الحصول على أو تعيين لغة واجهة المستخدم لإصدار المصنف بناءً على كود البلد الذي حفظ الملف.|
| [region](/cells/ar/python-net/aspose.cells/htmlloadoptions/region) | الحصول على أو تعيين الإعدادات الإقليمية للنظام بناءً على رمز البلد في وقت تحميل الملف.|
| [default_style_settings](/cells/ar/python-net/aspose.cells/htmlloadoptions/default_style_settings) | الحصول على إعدادات النمط الافتراضية لتهيئة أنماط المصنف|
| [standard_font](/cells/ar/python-net/aspose.cells/htmlloadoptions/standard_font) | يعيّن اسم الخط القياسي الافتراضي|
| [standard_font_size](/cells/ar/python-net/aspose.cells/htmlloadoptions/standard_font_size) | يعيّن حجم الخط القياسي الافتراضي.|
| [interrupt_monitor](/cells/ar/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) | يحصل على جهاز مراقبة المقاطعة ويضبطه.|
| [ignore_not_printed](/cells/ar/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) | تجاهل البيانات التي لم تتم طباعتها إذا قمت بطباعة الملف مباشرة|
| [check_data_valid](/cells/ar/python-net/aspose.cells/htmlloadoptions/check_data_valid) |تحقق مما إذا كانت البيانات صالحة في ملف القالب.|
| [check_excel_restriction](/cells/ar/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) | ما إذا كان التحقق من تقييد ملف Excel عند تعديل المستخدم للكائنات ذات الصلة بالخلايا.<br/>على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت.<br/>عند إدخال قيمة أطول من 32 كيلو بايت مثل Cell.PutValue (سلسلة) ، إذا كانت هذه الخاصية صحيحة ، فستحصل على استثناء.<br/>إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية حتى يتم ذلك لاحقًا<br/>يمكنك إخراج قيمة السلسلة الكاملة لتنسيقات ملفات أخرى مثل CSV.<br/>ومع ذلك ، إذا قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ،<br/> يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه.|
| [keep_unparsed_data](/cells/ar/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) | ما إذا كان سيتم الاحتفاظ بالبيانات التي لم يتم تحليلها في الذاكرة للمصنف عند تحميله من ملف القالب أم لا. الافتراضي هو الصحيح.|
| [load_filter](/cells/ar/python-net/aspose.cells/htmlloadoptions/load_filter) | عامل التصفية للدلالة على كيفية تحميل البيانات.|
| [light_cells_data_handler](/cells/ar/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب.|
| [memory_setting](/cells/ar/python-net/aspose.cells/htmlloadoptions/memory_setting) | الحصول على أو تعيين خيارات استخدام الذاكرة.|
| [warning_callback](/cells/ar/python-net/aspose.cells/htmlloadoptions/warning_callback) | يحصل أو يحدد رد الاتصال التحذيري.|
| [auto_fitter_options](/cells/ar/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) | الحصول على خيارات التركيب التلقائي وتعيينها|
| [auto_filter](/cells/ar/python-net/aspose.cells/htmlloadoptions/auto_filter) | يشير إلى ما إذا كانت التصفية التلقائية للبيانات عند تحميل الملفات.|
| [font_configs](/cells/ar/python-net/aspose.cells/htmlloadoptions/font_configs) | يحصل ويضبط تكوينات الخطوط الفردية.<br/> يعمل فقط مع [Workbook](/cells/ar/python-net/aspose.cells/workbook) الذي يستخدم [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions) للتحميل.|
| [encoding](/cells/ar/python-net/aspose.cells/htmlloadoptions/encoding) | الحصول على الترميز الافتراضي وتعيينه. ينطبق فقط على ملف csv.|
| [load_style_strategy](/cells/ar/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |يشير إلى إستراتيجية تطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ ووقت.|
| [convert_numeric_data](/cells/ar/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات رقمية.|
| [convert_date_time_data](/cells/ar/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات التاريخ.|
| [keep_precision](/cells/ar/python-net/aspose.cells/htmlloadoptions/keep_precision) | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان الطول 15.|
| [attached_files_directory](/cells/ar/python-net/aspose.cells/htmlloadoptions/attached_files_directory) | الدليل الذي سيتم حفظ الملفات المرفقة فيه.|
| [load_formulas](/cells/ar/python-net/aspose.cells/htmlloadoptions/load_formulas) | يشير إلى ما إذا كان استيراد الصيغ إذا كان ملف html الأصلي يحتوي على صيغ|
| [support_div_tag](/cells/ar/python-net/aspose.cells/htmlloadoptions/support_div_tag) | يشير إلى ما إذا كان يدعم تخطيط<div> علامة عندما يحتوي ملف html<div> العلامات. القيمة الافتراضية هي كاذبة.|
| [delete_redundant_spaces](/cells/ar/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) | الإشارة إلى ما إذا كان سيتم حذف المسافات الزائدة عند التفاف النص على الأسطر أم لا<br> العلامة ، القيمة الافتراضية هي false.|
| [auto_fit_cols_and_rows](/cells/ar/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) | يشير إلى ما إذا كان يتم احتواء الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي كاذبة.|
| [convert_formulas_data](/cells/ar/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) | إذا كانت القيمة صحيحة ، فقم بتحويل السلسلة إلى صيغة عندما تبدأ قيمة السلسلة بالحرف '=' ، فالقيمة الافتراضية هي false.|
| [stream_provider](/cells/ar/python-net/aspose.cells/htmlloadoptions/stream_provider) | الحصول على أو تعيين StreamProviderImportHtmlFile لاستيراد الكائنات.|
| [prog_id](/cells/ar/python-net/aspose.cells/htmlloadoptions/prog_id) | يحصل على معرف البرنامج الخاص بإنشاء الملف.<br/> فقط لملفات MHT.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_paper_size(type)](/cells/ar/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) | يضبط حجم ورق الطباعة الافتراضي من إعداد الطابعة الافتراضية.|



###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [AbstractTextLoadOptions](/cells/ar/python-net/aspose.cells/abstracttextloadoptions)
* فئة [HtmlLoadOptions](/cells/ar/python-net/aspose.cells/htmlloadoptions)
* فئة [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)
