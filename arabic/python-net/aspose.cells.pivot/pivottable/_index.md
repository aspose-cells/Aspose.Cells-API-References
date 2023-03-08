---
title: PivotTable الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  PivotTable الدرجة
وصف موجز لـ PivotTable.



يكشف نوع PivotTable الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_excel_2003_compatible](/cells/ar/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) | يحدد ما إذا كان PivotTable متوافقًا مع Excel2003 عند تحديث PivotTable ،<br/>إذا كان هذا صحيحًا ، يجب أن تكون السلسلة أقل من أو تساوي 255 حرفًا ، لذلك إذا كانت السلسلة أكبر من 255 حرفًا ،<br/>سيتم اقتطاعه. إذا كانت خاطئة ، فلن يكون للسلسلة القيود المذكورة أعلاه.<br/> القيمة الافتراضية هي الحقيقية.|
| [refreshed_by_who](/cells/ar/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) | الحصول على اسم المستخدم الذي قام بآخر تحديث لـ PivotTable|
| [refresh_date](/cells/ar/python-net/aspose.cells.pivot/pivottable/refresh_date) | الحصول على تاريخ آخر تحديث لـ PivotTable.|
| [pivot_table_style_name](/cells/ar/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) |الحصول على اسم النمط المحوري وتعيينه.|
| [pivot_table_style_type](/cells/ar/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) | الحصول على نمط الجدول المحوري المدمج وتعيينه.|
| [column_fields](/cells/ar/python-net/aspose.cells.pivot/pivottable/column_fields) | إرجاع كائن PivotFields الذي يتم عرضه حاليًا كحقول أعمدة.|
| [row_fields](/cells/ar/python-net/aspose.cells.pivot/pivottable/row_fields) |إرجاع كائن PivotFields الذي يتم عرضه حاليًا كحقول صفوف.|
| [page_fields](/cells/ar/python-net/aspose.cells.pivot/pivottable/page_fields) | إرجاع كائن PivotFields المعروض حاليًا كحقول صفحة.|
| [data_fields](/cells/ar/python-net/aspose.cells.pivot/pivottable/data_fields) | الحصول على كائن PivotField يمثل كافة حقول البيانات في PivotTable.<br/>للقراءة فقط ، سيتم البدء فقط في حالة وجود حقلي بيانات أو أكثر في DataPiovtFiels.<br/> يستخدم فقط لإضافة DataPivotField إلى منطقة صف / عمود PivotTable. الافتراضي في منطقة الصف.|
| [data_field](/cells/ar/python-net/aspose.cells.pivot/pivottable/data_field) | الحصول على كائن PivotField يمثل كافة حقول البيانات في PivotTable.<br/>للقراءة فقط ، سيتم البدء فقط في حالة وجود حقلي بيانات أو أكثر في DataPiovtFiels.<br/> يستخدم فقط لإضافة DataPivotField إلى منطقة صف / عمود PivotTable. الافتراضي في منطقة الصف.|
| [base_fields](/cells/ar/python-net/aspose.cells.pivot/pivottable/base_fields) | إرجاع كائن PivotFields يتضمن كافة الحقول في تقرير PivotTable|
| [pivot_filters](/cells/ar/python-net/aspose.cells.pivot/pivottable/pivot_filters) | إرجاع كائن PivotFilterCollection.|
| [column_range](/cells/ar/python-net/aspose.cells.pivot/pivottable/column_range) | إرجاع كائن CellArea يمثل النطاق<br/>الذي يحتوي على منطقة العمود في تقرير PivotTable. يقرأ فقط.|
| [row_range](/cells/ar/python-net/aspose.cells.pivot/pivottable/row_range) | إرجاع كائن CellArea يمثل النطاق<br/> الذي يحتوي على منطقة الصف في تقرير PivotTable. يقرأ فقط.|
| [data_body_range](/cells/ar/python-net/aspose.cells.pivot/pivottable/data_body_range) | إرجاع كائن CellArea الذي يمثل النطاق الذي يحتوي على منطقة البيانات<br/> في القائمة بين صف الرأس وصف الإدراج. يقرأ فقط.|
| [table_range1](/cells/ar/python-net/aspose.cells.pivot/pivottable/table_range1) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بأكمله ،<br/> لكنها لا تتضمن حقول الصفحة. يقرأ فقط.|
| [table_range2](/cells/ar/python-net/aspose.cells.pivot/pivottable/table_range2) | إرجاع كائن CellArea يمثل النطاق الذي يحتوي على تقرير PivotTable بأكمله ،<br/> يتضمن حقول الصفحة. يقرأ فقط.|
| [column_grand](/cells/ar/python-net/aspose.cells.pivot/pivottable/column_grand) | الإشارة إلى ما إذا كان تقرير PivotTable يعرض الإجماليات الكلية للأعمدة.|
| [is_grid_drop_zones](/cells/ar/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) | يشير إلى ما إذا كان تقرير PivotTable يعرض التخطيط الكلاسيكي المحوري.<br/> (يتيح سحب الحقول في الشبكة)|
| [row_grand](/cells/ar/python-net/aspose.cells.pivot/pivottable/row_grand) | الإشارة إلى ما إذا كان تقرير PivotTable يعرض الإجماليات الكلية للصفوف.|
| [display_null_string](/cells/ar/python-net/aspose.cells.pivot/pivottable/display_null_string) | الإشارة إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة<br/> في الخلايا التي تحتوي على قيم خالية.|
| [null_string](/cells/ar/python-net/aspose.cells.pivot/pivottable/null_string) | الحصول على السلسلة المعروضة في الخلايا التي تحتوي على قيم خالية<br/> عندما تكون الخاصية DisplayNullString صحيحة ، فالقيمة الافتراضية هي سلسلة فارغة.|
| [display_error_string](/cells/ar/python-net/aspose.cells.pivot/pivottable/display_error_string) | الإشارة إلى ما إذا كان تقرير PivotTable يعرض سلسلة مخصصة في الخلايا التي تحتوي على أخطاء.|
| [data_field_header_name](/cells/ar/python-net/aspose.cells.pivot/pivottable/data_field_header_name) | الحصول على اسم رأس حقل منطقة القيمة في PivotTable وتعيينه.|
| [error_string](/cells/ar/python-net/aspose.cells.pivot/pivottable/error_string) | الحصول على السلسلة المعروضة في الخلايا التي تحتوي على أخطاء<br/>عندما تكون الخاصية DisplayErrorString صحيحة ، فالقيمة الافتراضية هي سلسلة فارغة.|
| [is_auto_format](/cells/ar/python-net/aspose.cells.pivot/pivottable/is_auto_format) | الإشارة إلى ما إذا كان تقرير PivotTable قد تم تنسيقه تلقائيًا.<br/>حدد خانة الاختيار "جدول التنسيق التلقائي" الموجود في الخيار المحوري لبرنامج Excel 2003<br/> خانة الاختيار "احتواء تلقائي لعرض العمود عند التحديث" الموجود في خيارات الجدول المحوري: تنسيق التخطيط لبرنامج Excel 2007|
| [auto_format_type](/cells/ar/python-net/aspose.cells.pivot/pivottable/auto_format_type) | الحصول على نوع التنسيق التلقائي لـ PivotTable.|
| [has_blank_rows](/cells/ar/python-net/aspose.cells.pivot/pivottable/has_blank_rows) | يشير إلى ما إذا كان سيتم إضافة صفوف فارغة.<br/> تنطبق هذه الخاصية فقط على أنواع التنسيق التلقائي لـ PivotTable التي تحتاج إلى إضافة صفوف فارغة.|
| [merge_labels](/cells/ar/python-net/aspose.cells.pivot/pivottable/merge_labels) | الإشارة إلى ما إذا كان عنصر الصف الخارجي أو عنصر العمود أو الإجمالي الفرعي لتقرير PivotTable المحدد<br/> وتستخدم التسميات الإجمالية الكلية الخلايا المدمجة.|
| [preserve_formatting](/cells/ar/python-net/aspose.cells.pivot/pivottable/preserve_formatting) | الإشارة إلى ما إذا كان سيتم الاحتفاظ بالتنسيق عند تحديث PivotTable أو إعادة حسابه.|
| [show_drill](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_drill) | الحصول على ما إذا كان سيتم عرض أزرار التوسيع / الطي.|
| [enable_drilldown](/cells/ar/python-net/aspose.cells.pivot/pivottable/enable_drilldown) | يحصل على ما إذا كان التنقل لأسفل ممكّنًا أم لا.|
| [enable_field_dialog](/cells/ar/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) | يشير إلى ما إذا كان مربع الحوار حقل PivotTable متاحًا أم لا<br/> عندما ينقر المستخدم نقرًا مزدوجًا فوق حقل PivotTable.|
| [enable_field_list](/cells/ar/python-net/aspose.cells.pivot/pivottable/enable_field_list) | الحصول على ما إذا كان يتم تمكين قائمة الحقول لجدول PivotTable أم لا.|
| [enable_wizard](/cells/ar/python-net/aspose.cells.pivot/pivottable/enable_wizard) | الإشارة إلى ما إذا كان معالج PivotTable متاحًا أم لا.|
| [subtotal_hidden_page_items](/cells/ar/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) | الإشارة إلى ما إذا كانت عناصر حقل الصفحة المخفية موجودة في تقرير PivotTable أم لا<br/>يتم تضمينها في الإجماليات الفرعية للصفوف والأعمدة وإجماليات الكتل والإجماليات الكلية.<br/> القيمة الافتراضية هي كاذبة.|
| [grand_total_name](/cells/ar/python-net/aspose.cells.pivot/pivottable/grand_total_name) | تُرجع تسمية السلسلة النصية المعروضة في عمود الإجمالي الكلي أو عنوان الصف.<br/> القيمة الافتراضية هي السلسلة "الإجمالي الكلي".|
| [manual_update](/cells/ar/python-net/aspose.cells.pivot/pivottable/manual_update) | الإشارة إلى ما إذا كان سيتم إعادة حساب تقرير PivotTable بناءً على طلب المستخدم فقط.|
| [is_multiple_field_filters](/cells/ar/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) | تحدد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين عوامل تصفية متعددة على حقول PivotTable.|
| [missing_items_limit](/cells/ar/python-net/aspose.cells.pivot/pivottable/missing_items_limit) | تحدد قيمة منطقية تشير إلى ما إذا كان يمكن تعيين عوامل تصفية متعددة على حقول PivotTable.|
| [enable_data_value_editing](/cells/ar/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) |تحدد قيمة منطقية تشير إلى ما إذا كان المستخدم مسموحًا له بتحرير الخلايا في منطقة البيانات في المحور.<br/> قم بتمكين تحرير الخلية في منطقة القيم|
| [show_data_tips](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_data_tips) | تحدد قيمة منطقية تشير إلى ما إذا كان يجب عرض تلميحات الأدوات لخلايا بيانات PivotTable.|
| [show_member_property_tips](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) | تحدد قيمة منطقية تشير إلى ما إذا كان يجب حذف معلومات خصائص العضو من تلميحات أدوات PivotTable.|
| [show_values_row](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_values_row) | يحدد قيمة منطقية تشير إلى ما إذا كان سيتم إظهار صف القيم أم لا.<br/> إظهار صف القيم|
| [show_empty_col](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_empty_col) | يحدد قيمة منطقية تشير إلى ما إذا كان سيتم تضمين أعمدة فارغة في الجدول أم لا|
| [show_empty_row](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_empty_row) | تحدد قيمة منطقية تشير إلى ما إذا كان سيتم تضمين صفوف فارغة في الجدول أم لا.|
| [field_list_sort_ascending](/cells/ar/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) | تحدد قيمة منطقية تشير إلى ما إذا كان سيتم فرز الحقول في PivotTable بترتيب غير افتراضي في قائمة الحقول.|
| [print_drill](/cells/ar/python-net/aspose.cells.pivot/pivottable/print_drill) | يحدد قيمة منطقية تشير إلى ما إذا كان يجب طباعة مؤشرات الحفر.<br/> طباعة أزرار توسيع / طي عند عرضها على pivottable.|
| [alt_text_title](/cells/ar/python-net/aspose.cells.pivot/pivottable/alt_text_title) | يحصل على عنوان النص البديل|
| [alt_text_description](/cells/ar/python-net/aspose.cells.pivot/pivottable/alt_text_description) | يحصل على وصف النص البديل|
| [name](/cells/ar/python-net/aspose.cells.pivot/pivottable/name) | الحصول على اسم PivotTable|
| [column_header_caption](/cells/ar/python-net/aspose.cells.pivot/pivottable/column_header_caption) | الحصول على التسمية التوضيحية لرأس العمود في PivotTable.|
| [indent](/cells/ar/python-net/aspose.cells.pivot/pivottable/indent) | يحدد زيادة المسافة البادئة للمحور المضغوط ويمكن استخدامه لتعيين تخطيط التقرير إلى نموذج مضغوط.|
| [row_header_caption](/cells/ar/python-net/aspose.cells.pivot/pivottable/row_header_caption) | الحصول على التسمية التوضيحية لرأس الصف في PivotTable.|
| [show_row_header_caption](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) | الإشارة إلى ما إذا كان سيتم عرض التسمية التوضيحية لرأس الصف في تقرير PivotTable<br/> يشير إلى ما إذا كان يتم عرض تسميات الحقول وقوائم التصفية المنسدلة|
| [custom_list_sort](/cells/ar/python-net/aspose.cells.pivot/pivottable/custom_list_sort) | يشير إلى ما إذا كان يجب مراعاة القائمة المخصصة المضمنة عند فرز البيانات|
| [pivot_format_conditions](/cells/ar/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) | الحصول على شروط التنسيق للجدول المحوري.|
| [page_field_order](/cells/ar/python-net/aspose.cells.pivot/pivottable/page_field_order) |الحصول على الترتيب الذي تتم به إضافة حقول الصفحة إلى تخطيط تقرير PivotTable.|
| [page_field_wrap_count](/cells/ar/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) | الحصول على عدد حقول الصفحة في كل عمود أو صف في تقرير PivotTable.|
| [tag](/cells/ar/python-net/aspose.cells.pivot/pivottable/tag) | الحصول على سلسلة محفوظة بتقرير PivotTable.|
| [save_data](/cells/ar/python-net/aspose.cells.pivot/pivottable/save_data) | الإشارة إلى ما إذا كان سيتم حفظ بيانات تقرير PivotTable مع المصنف.|
| [refresh_data_on_opening_file](/cells/ar/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) | يشير إلى ما إذا كان سيتم تحديث البيانات عند فتح الملف.|
| [refresh_data_flag](/cells/ar/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) | يشير إلى تحديث البيانات أم لا.|
| [external_connection_data_source](/cells/ar/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) | يحصل على مصدر بيانات الاتصال الخارجي.|
| [data_source](/cells/ar/python-net/aspose.cells.pivot/pivottable/data_source) | الحصول على مصدر البيانات للجدول المحوري وتعيينه.|
| [item_print_titles](/cells/ar/python-net/aspose.cells.pivot/pivottable/item_print_titles) | بت يحدد ما إذا كانت تسميات توضيحية لعنصر محوري على محور الصف أم لا<br/> تتكرر في كل صفحة مطبوعة للحقول المحورية في شكل جدول.|
| [print_titles](/cells/ar/python-net/aspose.cells.pivot/pivottable/print_titles) | يشير إلى ما إذا كانت عناوين الطباعة لورقة العمل قد تم تعيينها على أساس<br/> في تقرير PivotTable. القيمة الافتراضية هي كاذبة.|
| [display_immediate_items](/cells/ar/python-net/aspose.cells.pivot/pivottable/display_immediate_items) | يشير إلى ما إذا كانت العناصر الموجودة في مناطق الصفوف والأعمدة مرئية أم لا<br/> عندما تكون منطقة البيانات في PivotTable فارغة. القيمة الافتراضية هي الحقيقية.|
| [is_selected](/cells/ar/python-net/aspose.cells.pivot/pivottable/is_selected) | الإشارة إلى ما إذا كان PivotTable محددًا أم لا.|
| [show_pivot_style_row_header](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) |يشير إلى ما إذا كان يجب تطبيق النمط على رأس الصف في الجدول المحوري.|
| [show_pivot_style_column_header](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) | يشير إلى ما إذا كان يجب تطبيق النمط على رأس العمود في الجدول المحوري.|
| [show_pivot_style_row_stripes](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) | الإشارة إلى ما إذا كان تنسيق شريط الصفوف مطبقًا أم لا.|
| [show_pivot_style_column_stripes](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا أم لا.|
| [show_pivot_style_last_column](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) | يشير إلى ما إذا كان تنسيق شريط العمود مطبقًا أم لا.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/ar/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) | يزيل حقلاً من منطقة حقل معينة|
| [remove_field(field_type, base_field_index)](/cells/ar/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) | يزيل حقلاً من منطقة حقل معينة|
| [remove_field(field_type, pivot_field)](/cells/ar/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) | إزالة الحقل من منطقة حقل معينة|
| [add_field_to_area(field_type, field_name)](/cells/ar/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) | يضيف الحقل إلى منطقة معينة.|
| [add_field_to_area(field_type, base_field_index)](/cells/ar/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) | يضيف الحقل إلى منطقة معينة.|
| [add_field_to_area(field_type, pivot_field)](/cells/ar/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) | يضيف الحقل إلى منطقة معينة.|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/ar/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) | يضيف حقلاً محسوبًا إلى الحقل المحوري.|
| [add_calculated_field(name, formula)](/cells/ar/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) |يضيف حقلاً محسوبًا إلى الحقل المحوري واسحبه إلى منطقة البيانات.|
| [move(row, column)](/cells/ar/python-net/aspose.cells.pivot/pivottable/move/#int-int) | نقل PivotTable إلى موقع مختلف في ورقة العمل.|
| [move(dest_cell_name)](/cells/ar/python-net/aspose.cells.pivot/pivottable/move/#str) | نقل PivotTable إلى موقع مختلف في ورقة العمل.|
| [set_auto_group_field(base_field_index)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) | يعيّن مجموعة الحقول التلقائية بواسطة PivotTable.|
| [set_auto_group_field(pivot_field)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) | يعيّن مجموعة الحقول التلقائية بواسطة PivotTable.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) | يعيّن مجموعة الحقول اليدوية بواسطة PivotTable.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) | يعيّن مجموعة الحقول اليدوية بواسطة PivotTable.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) | يعيّن مجموعة الحقول اليدوية بواسطة PivotTable.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) | يعيّن مجموعة الحقول اليدوية بواسطة PivotTable.|
| [set_ungroup(base_field_index)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) | يعين فك التجميع بواسطة PivotTable|
| [set_ungroup(pivot_field)](/cells/ar/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) | يعين فك التجميع بواسطة PivotTable|
| [copy_style(pivot_table)](/cells/ar/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) | نسخ نمط مسمى من جدول محوري آخر.|
| [show_report_filter_page(page_field)](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) | إظهار كافة صفحات عامل تصفية التقرير وفقًا لـ PivotField ، يجب أن يكون PivotField موجودًا في PageFields.|
| [show_report_filter_page_by_name(field_name)](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) | إظهار كافة صفحات عامل تصفية التقرير وفقًا لاسم PivotField ، يجب أن يكون PivotField موجودًا في PageFields.|
| [show_report_filter_page_by_index(pos_index)](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) | إظهار كافة صفحات تصفية التقرير وفقًا لفهرس الموضع في PageFields|
| [fields(field_type)](/cells/ar/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) | يحصل على الحقول المحددة حسب نوع الحقل.|
| [change_data_source(source)](/cells/ar/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) |تعيين مصدر البيانات المحورية.<br/> الورقة 1! $ A $ 1: $ C $ 3|
| [get_source()](/cells/ar/python-net/aspose.cells.pivot/pivottable/get_source/#) | احصل على بيانات مصدر pivottable.|
| [refresh_data()](/cells/ar/python-net/aspose.cells.pivot/pivottable/refresh_data/#) | تحديث بيانات pivottable والإعداد من مصدر البيانات الخاص به.|
| [calculate_data()](/cells/ar/python-net/aspose.cells.pivot/pivottable/calculate_data/#) | تحسب بيانات pivottable إلى الخلايا.|
| [clear_data()](/cells/ar/python-net/aspose.cells.pivot/pivottable/clear_data/#) | امسح بيانات وتنسيق PivotTable|
| [calculate_range()](/cells/ar/python-net/aspose.cells.pivot/pivottable/calculate_range/#) | يحسب نطاق pivottable.|
| [format_all(style)](/cells/ar/python-net/aspose.cells.pivot/pivottable/format_all/#Style) | قم بتنسيق كل الخلايا في المنطقة المحورية|
| [format_row(row, style)](/cells/ar/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) | قم بتنسيق بيانات الصف في المنطقة المحورية|
| [format(row, column, style)](/cells/ar/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) | قم بتنسيق الخلية في المنطقة المحورية|
| [get_horizontal_breaks()](/cells/ar/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) | الحصول على قائمة فهرس صف الجدول المحوري بفواصل الصفحات الأفقية|
| [show_in_compact_form()](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) |تخطيطات PivotTable في شكل مضغوط.|
| [show_in_outline_form()](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) | تخطيطات PivotTable في نموذج المخطط التفصيلي.|
| [show_in_tabular_form()](/cells/ar/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) | تخطيطات PivotTable في شكل جدولي.|
| [get_cell_by_display_name(display_name)](/cells/ar/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) | يحصل على العنصر Cell بواسطة DisplayName الخاص بـ PivotField|
| [get_children()](/cells/ar/python-net/aspose.cells.pivot/pivottable/get_children/#) |الحصول على جداول الأطفال المحورية التي تستخدم بيانات PivotTable هذه كمصدر بيانات.|



###  مثال

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  أنظر أيضا
* وحدة [aspose.cells.pivot](..)
