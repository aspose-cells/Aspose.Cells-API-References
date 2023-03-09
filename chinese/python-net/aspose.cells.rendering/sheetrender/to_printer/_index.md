---
title: to_printer方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells.rendering/sheetrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
将工作表渲染到打印机



```python
def to_printer(self, printer_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| printer_name | str |打印机的名称，例如：“Microsoft Office Document Image Writer”|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
将工作表渲染到打印机



```python
def to_printer(self, printer_settings):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings |打印机的设置，例如 PrinterName、Duplex|


##  to_printer(printer_name, job_name) {#str-str}
将工作表渲染到打印机



```python
def to_printer(self, printer_name, job_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| printer_name | str |打印机的名称，例如：“Microsoft Office Document Image Writer”|
| job_name | str |设置打印作业名称|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
将工作表渲染到打印机



```python
def to_printer(self, printer_settings, job_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings |打印机的设置，例如 PrinterName、Duplex|
| job_name | str |设置打印作业名称|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
将工作表渲染到打印机



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| printer_name | str |打印机的名称，例如：“Microsoft Office Document Image Writer”|
| print_page_index | int |要打印的第一页从 0 开始的索引，它必须在范围 [0, SheetRender.PageCount-1] 内|
| print_page_count | int |要打印的页数，它必须大于零|
### 评论

注意：此方法现已过时。
相反，请使用 ToPrinter(string PrinterName) 和 ImageOrPrintOptions.PageIndex, PageCount 来设置第一页和要打印的页数。
自 2021 年 12 月起，此属性将在 12 个月后移除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells.rendering](../../)
* 类 [SheetRender](/cells/zh/python-net/aspose.cells.rendering/sheetrender)
