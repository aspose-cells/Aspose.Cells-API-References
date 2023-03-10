---
title: TxtLoadOptions الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 1510
url: /ar/python-net/aspose.cells/txtloadoptions/
is_root: false
---
##  TxtLoadOptions الدرجة
يمثل خيارات تحميل ملف نصي.



**ميراث:** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions)



يكشف نوع TxtLoadOptions الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [TxtLoadOptions()](/cells/ar/python-net/aspose.cells/txtloadoptions/__init__/#) | ينشئ خيارات لتحميل ملف نصي.|
| [TxtLoadOptions(load_format)](/cells/ar/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) | ينشئ خيارات لتحميل ملف نصي.|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [load_format](/cells/ar/python-net/aspose.cells/txtloadoptions/load_format) | يحصل على تنسيق التحميل.|
| [password](/cells/ar/python-net/aspose.cells/txtloadoptions/password) | الحصول على كلمة المرور الخاصة بالمصنف وتعيينها.|
| [parsing_formula_on_open](/cells/ar/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) | يشير إلى ما إذا كان سيتم تحليل الصيغة عند قراءة الملف.|
| [parsing_pivot_cached_records](/cells/ar/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) | يشير إلى ما إذا كان تحليل السجلات المحورية المخزنة مؤقتًا عند تحميل الملف.<br/> القيمة الافتراضية هي كاذبة.|
| [language_code](/cells/ar/python-net/aspose.cells/txtloadoptions/language_code) | الحصول على أو تعيين لغة واجهة المستخدم لإصدار المصنف بناءً على كود البلد الذي حفظ الملف.|
| [region](/cells/ar/python-net/aspose.cells/txtloadoptions/region) | الحصول على أو تعيين الإعدادات الإقليمية للنظام بناءً على رمز البلد في وقت تحميل الملف.|
| [default_style_settings](/cells/ar/python-net/aspose.cells/txtloadoptions/default_style_settings) | الحصول على إعدادات النمط الافتراضية لتهيئة أنماط المصنف|
| [standard_font](/cells/ar/python-net/aspose.cells/txtloadoptions/standard_font) | يعيّن اسم الخط القياسي الافتراضي|
| [standard_font_size](/cells/ar/python-net/aspose.cells/txtloadoptions/standard_font_size) | يعيّن حجم الخط القياسي الافتراضي.|
| [interrupt_monitor](/cells/ar/python-net/aspose.cells/txtloadoptions/interrupt_monitor) | يحصل على جهاز مراقبة المقاطعة ويضبطه.|
| [ignore_not_printed](/cells/ar/python-net/aspose.cells/txtloadoptions/ignore_not_printed) | تجاهل البيانات التي لم تتم طباعتها إذا قمت بطباعة الملف مباشرة|
| [check_data_valid](/cells/ar/python-net/aspose.cells/txtloadoptions/check_data_valid) |تحقق مما إذا كانت البيانات صالحة في ملف القالب.|
| [check_excel_restriction](/cells/ar/python-net/aspose.cells/txtloadoptions/check_excel_restriction) | ما إذا كان التحقق من تقييد ملف Excel عند تعديل المستخدم للكائنات ذات الصلة بالخلايا.<br/>على سبيل المثال ، لا يسمح Excel بإدخال قيمة سلسلة أطول من 32 كيلو بايت.<br/>عند إدخال قيمة أطول من 32 كيلو بايت مثل Cell.PutValue (سلسلة) ، إذا كانت هذه الخاصية صحيحة ، فستحصل على استثناء.<br/>إذا كانت هذه الخاصية خاطئة ، فسنقبل قيمة سلسلة الإدخال كقيمة للخلية حتى يتم ذلك لاحقًا<br/>يمكنك إخراج قيمة السلسلة الكاملة لتنسيقات ملفات أخرى مثل CSV.<br/>ومع ذلك ، إذا قمت بتعيين مثل هذا النوع من القيمة غير الصالحة لتنسيق ملف Excel ،<br/> يجب ألا تحفظ المصنف بتنسيق ملف excel لاحقًا. وإلا فقد يكون هناك خطأ غير متوقع لملف Excel الذي تم إنشاؤه.|
| [keep_unparsed_data](/cells/ar/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) | ما إذا كان سيتم الاحتفاظ بالبيانات التي لم يتم تحليلها في الذاكرة للمصنف عند تحميله من ملف القالب أم لا. الافتراضي هو الصحيح.|
| [load_filter](/cells/ar/python-net/aspose.cells/txtloadoptions/load_filter) | عامل التصفية للدلالة على كيفية تحميل البيانات.|
| [light_cells_data_handler](/cells/ar/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) | معالج البيانات لمعالجة بيانات الخلايا عند قراءة ملف القالب.|
| [memory_setting](/cells/ar/python-net/aspose.cells/txtloadoptions/memory_setting) | الحصول على أو تعيين خيارات استخدام الذاكرة.|
| [warning_callback](/cells/ar/python-net/aspose.cells/txtloadoptions/warning_callback) | يحصل أو يحدد رد الاتصال التحذيري.|
| [auto_fitter_options](/cells/ar/python-net/aspose.cells/txtloadoptions/auto_fitter_options) | الحصول على خيارات التركيب التلقائي وتعيينها|
| [auto_filter](/cells/ar/python-net/aspose.cells/txtloadoptions/auto_filter) | يشير إلى ما إذا كانت التصفية التلقائية للبيانات عند تحميل الملفات.|
| [font_configs](/cells/ar/python-net/aspose.cells/txtloadoptions/font_configs) | يحصل ويضبط تكوينات الخطوط الفردية.<br/> يعمل فقط مع [Workbook](/cells/ar/python-net/aspose.cells/workbook) الذي يستخدم [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions) للتحميل.|
| [encoding](/cells/ar/python-net/aspose.cells/txtloadoptions/encoding) | الحصول على الترميز الافتراضي وتعيينه. ينطبق فقط على ملف csv.|
| [load_style_strategy](/cells/ar/python-net/aspose.cells/txtloadoptions/load_style_strategy) |يشير إلى إستراتيجية تطبيق النمط على القيم التي تم تحليلها عند تحويل قيمة السلسلة إلى رقم أو تاريخ ووقت.|
| [convert_numeric_data](/cells/ar/python-net/aspose.cells/txtloadoptions/convert_numeric_data) | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات رقمية.|
| [convert_date_time_data](/cells/ar/python-net/aspose.cells/txtloadoptions/convert_date_time_data) | الحصول على أو تعيين قيمة تشير إلى ما إذا كانت السلسلة في ملف نصي قد تم تحويلها إلى بيانات التاريخ.|
| [keep_precision](/cells/ar/python-net/aspose.cells/txtloadoptions/keep_precision) | يشير إلى ما إذا كان لا يتم تحليل قيمة سلسلة إذا كان الطول 15.|
| [separator](/cells/ar/python-net/aspose.cells/txtloadoptions/separator) | يحصل ويضبط فاصل الأحرف لملف نصي.|
| [separator_string](/cells/ar/python-net/aspose.cells/txtloadoptions/separator_string) | الحصول على قيمة سلسلة وتعيينها كفاصل.|
| [is_multi_encoded](/cells/ar/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | يعني صحيح أن الملف يحتوي على عدة ترميزات.|
| [preferred_parsers](/cells/ar/python-net/aspose.cells/txtloadoptions/preferred_parsers) |الحصول على وتعيين محللات القيمة المفضلة لتحميل ملف نصي.|
| [has_formula](/cells/ar/python-net/aspose.cells/txtloadoptions/has_formula) | يشير إلى ما إذا كان النص صيغة إذا كان يبدأ بـ "=".|
| [has_text_qualifier](/cells/ar/python-net/aspose.cells/txtloadoptions/has_text_qualifier) | ما إذا كان هناك مؤهل نص لقيمة الخلية. الافتراضي هو الصحيح.|
| [text_qualifier](/cells/ar/python-net/aspose.cells/txtloadoptions/text_qualifier) | يحدد مؤهل النص لقيم الخلية. المؤهل الافتراضي هو '"'.|
| [treat_consecutive_delimiters_as_one](/cells/ar/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) | ما إذا كان يجب التعامل مع المحددات المتتالية على أنها واحدة.|
| [treat_quote_prefix_as_value](/cells/ar/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) | يشير إلى ما إذا كان يجب أخذ علامة الاقتباس المفردة كجزء من قيمة خلية واحدة.<br/>الافتراضي هو الصحيح. إذا كانت خاطئة ، فستتم إزالة علامة الاقتباس المفردة البادئة من قيمة الخلية المقابلة<br/> وسيتم تعيين [Style.quote_prefix](/cells/ar/python-net/aspose.cells/style#quote_prefix) على أنه صحيح للخلية.|
| [extend_to_next_sheet](/cells/ar/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) | ما إذا كان يوسع البيانات إلى الورقة التالية عندما تتجاوز صفوف أو أعمدة البيانات الحد.<br/>إذا كانت هذه الخاصية صحيحة ، فسيتم تمديد البيانات الإضافية إلى الورقة التالية خلف الورقة الحالية (إذا كانت الورقة الحالية هي الأخيرة ،<br/>سيتم إلحاق ورقة جديدة بالمصنف الحالي).<br/>إذا كانت هذه الخاصية خاطئة ، فسيتم تجاهل البيانات التي تتجاوز الحد.<br/> الافتراضي هو خطأ.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_paper_size(type)](/cells/ar/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) | يضبط حجم ورق الطباعة الافتراضي من إعداد الطابعة الافتراضية.|



###  أنظر أيضا
* وحدة [aspose.cells](..)
* فئة [AbstractTextLoadOptions](/cells/ar/python-net/aspose.cells/abstracttextloadoptions)
* فئة [LoadOptions](/cells/ar/python-net/aspose.cells/loadoptions)
* فئة [TxtLoadOptions](/cells/ar/python-net/aspose.cells/txtloadoptions)
* فئة [Workbook](/cells/ar/python-net/aspose.cells/workbook)
