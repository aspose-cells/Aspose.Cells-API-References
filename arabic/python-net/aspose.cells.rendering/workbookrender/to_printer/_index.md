---
title: طريقة to_printer
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 50
url: /ar/python-net/aspose.cells.rendering/workbookrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
تقديم المصنف إلى الطابعة



```python
def to_printer(self, printer_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| printer_name | str | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
تقديم المصنف إلى الطابعة



```python
def to_printer(self, printer_settings):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | إعدادات الطابعة ، على سبيل المثال اسم الطابعة ، الطباعة على الوجهين|


##  to_printer(printer_name, job_name) {#str-str}
تقديم المصنف إلى الطابعة



```python
def to_printer(self, printer_name, job_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| printer_name | str | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer"|
| job_name | str | قم بتعيين اسم مهمة الطباعة|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
تقديم المصنف إلى الطابعة



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | إعدادات الطابعة ، على سبيل المثال اسم الطابعة ، الطباعة على الوجهين|
| job_name | str | قم بتعيين اسم مهمة الطباعة|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
تقديم المصنف إلى الطابعة



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| printer_name | str | اسم الطابعة ، على سبيل المثال: "Microsoft Office Document Image Writer"|
| print_page_index | int | الفهرس الذي يستند إلى 0 للصفحة الأولى للطباعة ، يجب أن يكون في النطاق [0 ، WorkbookRender.PageCount-1]|
| print_page_count | int | عدد الصفحات المراد طباعتها ، يجب أن يكون أكبر من الصفر|
###  ملاحظات

ملاحظة: هذه الطريقة عفا عليها الزمن الآن.
بدلاً من ذلك ، يرجى استخدام ToPrinter (سلسلة PrinterName) و ImageOrPrintOptions.PageIndex و PageCount لتعيين الصفحة الأولى وعدد الصفحات المطلوب طباعتها.
 ستتم إزالة هذا العقار بعد 12 شهرًا منذ ديسمبر 2021.
Aspose يعتذر عن أي إزعاج قد يكون سببه لك.


###  أنظر أيضا
* وحدة [aspose.cells.rendering](../../)
* فئة [WorkbookRender](/cells/ar/python-net/aspose.cells.rendering/workbookrender)
