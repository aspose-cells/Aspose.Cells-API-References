---
title: SheetRender الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 100
url: /ar/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender الدرجة
يمثل عرض ورقة عمل يمكن أن يعرض ورقة العمل على صور مختلفة مثل (BMP ، PNG ، JPEG ، TIFF ..)
يجب استخدام مُنشئ هذه الفئة بعد تعديل إعداد الصفحات ونمط الخلية.



يكشف نوع SheetRender الأعضاء التالية:

###  المنشئون
| البناء| وصف|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | بناء SheetRender ، تحتاج إلى ورقة عمل و ImageOrPrintOptions كمعلمات|


###  ملكيات
| ملكية| وصف|
| :- | :- |
| [page_count](/cells/ar/python-net/aspose.cells.rendering/sheetrender/page_count) | الحصول على إجمالي عدد الصفحات لورقة العمل الحالية.|
| [page_scale](/cells/ar/python-net/aspose.cells.rendering/sheetrender/page_scale) | يحصل على مقياس الصفحة المحسوب للورقة.<br/> إرجاع المقياس المحدد إذا تم تعيين [PageSetup.zoom](/cells/ar/python-net/aspose.cells/pagesetup#zoom). وإلا ، تُرجع المقياس المحسوب وفقًا لـ [PageSetup.fit_to_pages_wide](/cells/ar/python-net/aspose.cells/pagesetup#fit_to_pages_wide) و [PageSetup.fit_to_pages_tall](/cells/ar/python-net/aspose.cells/pagesetup#fit_to_pages_tall).|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [to_image(page_index, file_name)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | تقديم صفحة معينة إلى ملف.|
| [to_image(page_index, stream)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | تقديم صفحة معينة إلى دفق.|
| [to_tiff(stream)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | عرض ورقة العمل بأكملها على شكل Tiff Image للدفق.|
| [to_tiff(filename)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | تقديم ورقة العمل بأكملها على شكل Tiff Image إلى ملف.|
| [to_printer(printer_name)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | تقديم ورقة العمل للطابعة|
| [to_printer(printer_name, job_name)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | تقديم ورقة العمل للطابعة|
| [to_printer(printer_settings)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | تقديم ورقة العمل للطابعة|
| [to_printer(printer_settings, job_name)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | تقديم ورقة العمل للطابعة|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | تقديم ورقة العمل للطابعة|
| [get_page_size_inch(page_index)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |الحصول على حجم الصفحة بوصة من الصورة الناتجة.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/ar/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | يمكن للعميل التحكم في إعداد صفحة الطابعة عند طباعة كل صفحة باستخدام هذه الوظيفة.|



###  أنظر أيضا
* وحدة [aspose.cells.rendering](..)
