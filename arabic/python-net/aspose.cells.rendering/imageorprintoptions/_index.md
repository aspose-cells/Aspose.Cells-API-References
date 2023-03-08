---
title: ImageOrPrintOptions الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 40
url: /ar/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions الدرجة
يسمح بتحديد الخيارات عند عرض ورقة العمل على الصور أو طباعة ورقة العمل أو عرض الرسم البياني على الصورة.



يكشف نوع ImageOrPrintOptions الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [ImageOrPrintOptions()](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | إنشاء مثيل جديد من ImageOrPrintOptions|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [save_format](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | الحصول على نوع تنسيق ملف الإخراج أو تحديده<br/> دعم Tiff / XPS|
| [print_with_status_dialog](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | إذا كانت PrintWithStatusDialog = true ، فسيكون هناك مربع حوار يعرض حالة الطباعة الحالية.<br/> وإلا لن يظهر مثل هذا الحوار.|
| [horizontal_resolution](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) |الحصول على الدقة الأفقية أو ضبطها للصور المُنشأة ، بالنقاط في البوصة.<br/> يطبق طريقة إنشاء الصورة باستثناء الصور بتنسيق Emf.|
| [vertical_resolution](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | الحصول على الدقة الرأسية للصور المُنشأة أو تعيينها ، بالنقاط في البوصة.<br/> يطبق طريقة إنشاء الصورة باستثناء صورة بتنسيق Emf.|
| [tiff_compression](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | الحصول على أو تحديد نوع الضغط ليتم تطبيقه فقط عند حفظ الصفحات بتنسيق `Tiff`.|
| [tiff_color_depth](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | الحصول على عمق البت أو تعيينه ليتم تطبيقه فقط عند حفظ الصفحات بتنسيق `Tiff`.|
| [printing_page](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | يشير إلى الصفحات التي لن تتم طباعتها.|
| [quality](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/quality) | الحصول على أو تحديد قيمة تحدد جودة الصور المُنشأة<br/> لتطبيقه فقط عند حفظ الصفحات بتنسيق `Jpeg`. القيمة الافتراضية هي 100|
| [image_type](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | الحصول على أو تحديد تنسيق الصور التي تم إنشاؤها.<br/> القيمة الافتراضية: PNG.|
| [is_cell_auto_fit](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | يشير إلى ما إذا كان عرض الخلايا وارتفاعها يتناسب تلقائيًا مع قيمة الخلية.<br/> القيمة الافتراضية هي كاذبة.|
| [one_page_per_sheet](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | إذا كانت OnePagePerSheet صحيحة ، فسيتم إخراج كل محتوى ورقة واحدة إلى صفحة واحدة فقط نتيجة لذلك.<br/> سيكون حجم الورق الخاص بإعداد الصفحات غير صالح ، والإعدادات الأخرى لإعداد الصفحات<br/> ستظل نافذة المفعول.|
| [all_columns_in_one_page_per_sheet](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | إذا كانت AllColumnsInOnePagePerSheet صحيحة ، فسيتم إخراج محتوى العمود بالكامل في ورقة واحدة إلى صفحة واحدة فقط في النتيجة.<br/> سيكون عرض حجم الورق الخاص بإعداد الصفحات غير صالح ، والإعدادات الأخرى لإعداد الصفحات<br/> ستظل نافذة المفعول.|
| [draw_object_event_handler](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | تنفذ هذه الواجهة للحصول على DrawObject و Bound عند العرض.|
| [chart_image_type](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | أشر إلى نوع الرسم البياني عند التحويل.<br/> القيمة الافتراضية: PNG.|
| [embeded_image_name_in_svg](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | أشر إلى اسم ملف الصورة المضمنة بتنسيق svg.<br/> يجب أن يكون هذا المسار كاملًا مع دليل مثل "c: \\ xpsEmbedded"|
| [svg_fit_to_view_port](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | إذا كانت هذه الخاصية صحيحة ، فسيكون svg الذي تم إنشاؤه مناسبًا لعرض المنفذ.|
| [only_area](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | إذا كانت هذه الخاصية صحيحة ، فسيتم إخراج منطقة واحدة ، ولن يسري أي مقياس.|
| [text_rendering_hint](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | يحدد جودة عرض النص.<br/> القيمة الافتراضية هي TextRenderingHint.SystemDefault|
| [smoothing_mode](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | يحدد ما إذا كان التنعيم (مضاد الحواف) مطبقًا على الخطوط والمنحنيات وحواف المساحات المعبأة.<br/> القيمة الافتراضية هي SmoothingMode.None|
| [transparent](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | يشير إلى ما إذا كانت خلفية الصورة التي تم إنشاؤها يجب أن تكون شفافة.|
| [pixel_format](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) | الحصول على أو تحديد تنسيق البكسل للصور التي تم إنشاؤها.|
| [warning_callback](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | يحصل أو يحدد رد الاتصال التحذيري.|
| [page_saving_callback](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) |التحكم / الإشارة إلى التقدم المحرز في عملية حفظ الصفحة.|
| [is_font_substitution_char_granularity](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | الإشارة إلى ما إذا كان سيتم استبدال خط الحرف فقط عندما لا يكون خط الخلية متوافقًا معه.|
| [page_index](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | الحصول على أو تحديد الفهرس الذي يستند إلى 0 للصفحة الأولى لحفظها.|
| [page_count](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | الحصول على أو تحديد عدد الصفحات المراد حفظها.|
| [is_optimized](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | يشير إلى ما إذا كان سيتم تحسين عناصر الإخراج.|
| [default_font](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ،<br/>قد تظهر على شكل كتلة في صورة pdf.<br/>قم بتعيين الخط الافتراضي مثل MingLiu أو MS Gothic لإظهار هذه الأحرف.<br/> إذا لم يتم تعيين هذه الخاصية ، فسيستخدم Aspose.Cells الخط الافتراضي للنظام لإظهار أحرف unicode هذه.|
| [check_workbook_default_font](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | عندما تكون الأحرف في Excel Unicode ولا يتم تعيينها بالخط الصحيح في نمط الخلية ،<br/>قد تظهر على شكل كتلة في صورة pdf.<br/> اضبط هذا على صواب لمحاولة استخدام الخط الافتراضي للمصنف لإظهار هذه الأحرف أولاً.|
| [output_blank_page_when_nothing_to_print](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | يشير إلى ما إذا كان سيتم إخراج صفحة فارغة في حالة عدم وجود شيء للطباعة.|
| [gridline_type](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | الحصول على نوع خط الشبكة أو تعيينه.|
| [text_cross_type](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | الحصول على عرض نوع النص أو تعيينه عندما يكون عرض النص أكبر من عرض الخلية.|
| [emf_type](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | الحصول على أو تعيين EmfType الذي يحدد تنسيق ملف التعريف ..<br/>القيمة الافتراضية هي EmfPlusDual.|
| [default_edit_language](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | الحصول على أو تعيين لغة التحرير الافتراضية.|
| [sheet_set](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |الحصول على الأوراق أو تعيينها للعرض. الافتراضي هو كل الأوراق المرئية في المصنف: [SheetSet.visible](/cells/ar/python-net/aspose.cells.rendering/sheetset#visible).|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/ar/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | يضبط العرض والارتفاع المطلوبين للصورة.|



###  مثال

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  أنظر أيضا
* وحدة [aspose.cells.rendering](..)
