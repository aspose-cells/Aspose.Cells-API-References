---
title: CellsHelper الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 230
url: /ar/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper الدرجة
يوفر وظائف المساعد.



يكشف نوع CellsHelper الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [significant_digits](/cells/ar/python-net/aspose.cells/cellshelper/significant_digits) | الحصول على عدد الخانات المعنوية وتعيينها.<br/> القيمة الافتراضية هي 17.|
| [dpi](/cells/ar/python-net/aspose.cells/cellshelper/dpi) | يحصل على DPI للجهاز.|
| [startup_path](/cells/ar/python-net/aspose.cells/cellshelper/startup_path) |الحصول على أو تعيين مسار بدء التشغيل ، والذي يشار إليه ببعض مراجع الصيغ الخارجية.|
| [alt_start_path](/cells/ar/python-net/aspose.cells/cellshelper/alt_start_path) | الحصول على أو تعيين مسار بدء التشغيل البديل ، والذي يشار إليه بواسطة بعض مراجع الصيغ الخارجية.|
| [library_path](/cells/ar/python-net/aspose.cells/cellshelper/library_path) | الحصول على أو تعيين مسار المكتبة المشار إليه ببعض مراجع الصيغ الخارجية.|
| [custom_implementation_factory](/cells/ar/python-net/aspose.cells/cellshelper/custom_implementation_factory) | الحصول على المصنع أو تعيينه لإنشاء مثيلات ذات تنفيذ خاص.|
| [is_cloud_platform](/cells/ar/python-net/aspose.cells/cellshelper/is_cloud_platform) | يرجى ضبط هذه الخاصية على True عند التشغيل على منصة سحابية ، مثل: Azure و AWSLambda وما إلى ذلك ،|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/ar/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | للتحقق من اسم الورقة المحدد وإنشاء اسم صالح عند الحاجة.<br/>إذا كان اسم الورقة المعطى يتوافق مع قواعد اسم ورقة Excel ، فقم بإعادتها.<br/>وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد<br/> وسيتم استبدال الأحرف غير الصالحة بـ "" ، ثم يتم إرجاع قيمة السلسلة المعاد بناؤها.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/ar/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | للتحقق من اسم الورقة المحدد وإنشاء اسم صالح عند الحاجة.<br/>إذا كان اسم الورقة المعطى يتوافق مع قواعد اسم ورقة Excel ، فقم بإعادتها.<br/>وإلا سيتم قطع السلسلة إذا تجاوز الطول الحد<br/> وسيتم استبدال الأحرف غير الصالحة بحرف معين ، ثم إرجاع قيمة السلسلة المعاد بناؤها.|
| [get_text_width(text, font, scaling)](/cells/ar/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | احصل على عرض النص بوحدة من النقاط.|
| [get_version()](/cells/ar/python-net/aspose.cells/cellshelper/get_version/#) | احصل على نسخة الإصدار.|
| [cell_name_to_index(cell_name, row, column)](/cells/ar/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | الحصول على فهارس صف الخلية والأعمدة وفقًا لاسمها.|
| [cell_index_to_name(row, column)](/cells/ar/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | الحصول على اسم الخلية وفقًا لفهارس الصفوف والأعمدة.|
| [column_index_to_name(column)](/cells/ar/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | يحصل على اسم العمود وفقا لفهرس العمود.|
| [column_name_to_index(column_name)](/cells/ar/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |يحصل على فهرس العمود وفقًا لاسم العمود.|
| [row_index_to_name(row)](/cells/ar/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | يحصل على اسم الصف وفقا لفهرس الصف.|
| [row_name_to_index(row_name)](/cells/ar/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | يحصل على فهرس الصف وفقا لاسم الصف.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/ar/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | لتحويل صيغة r1c1 للخلية إلى صيغة A1.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/ar/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | يحول صيغة A1 للخلية إلى صيغة r1c1.|
| [get_date_time_from_double(double_value, date1904)](/cells/ar/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | تحويل القيمة المزدوجة إلى قيمة وقت التاريخ.|
| [get_double_from_date_time(date_time, date1904)](/cells/ar/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | تحويل وقت التاريخ إلى قيمة مضاعفة.|
| [get_used_colors(workbook)](/cells/ar/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | يحصل على كل الألوان المستخدمة في المصنف.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/ar/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | أضف وظيفة الوظيفة الإضافية.|
| [merge_files(files, cached_file, dest_file)](/cells/ar/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | يدمج بعض ملفات xls الكبيرة في ملف xls.|
| [init_for_dot_net_core()](/cells/ar/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | قم بالتهيئة لبرنامج .NetCore.<br/> نقترح عليك استدعاء هذه الطريقة للجميع تهيئة NetCore أولاً.<br/>على سبيل المثال:<br/>CellsHelper.InitForDotNetCore () ،<br/> المصنف wb = مصنف جديد () ؛|



###  أنظر أيضا
* وحدة [aspose.cells](..)
