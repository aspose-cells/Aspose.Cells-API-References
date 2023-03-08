---
title: SheetRender类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender类
表示一个工作表渲染器，它可以将工作表渲染成各种图像，例如 (BMP, PNG, JPEG, TIFF..)
该类的构造函数，必须在pagesetup、cell style修改后使用。



SheetRender 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | SheetRender 的构造，需要工作表和 ImageOrPrintOptions 作为参数|


### 特性
|属性|描述|
| :- | :- |
| [page_count](/cells/zh/python-net/aspose.cells.rendering/sheetrender/page_count) |获取当前工作表的总页数。|
| [page_scale](/cells/zh/python-net/aspose.cells.rendering/sheetrender/page_scale) |获取工作表的计算页面比例。<br/>如果设置了 [PageSetup.zoom](/cells/zh/python-net/aspose.cells/pagesetup#zoom)，则返回设置的比例。否则返回根据[PageSetup.fit_to_pages_wide](/cells/zh/python-net/aspose.cells/pagesetup#fit_to_pages_wide)和[PageSetup.fit_to_pages_tall](/cells/zh/python-net/aspose.cells/pagesetup#fit_to_pages_tall)计算出的比例。|


### 方法
|方法|描述|
| :- | :- |
| [to_image(page_index, file_name)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) |将特定页面渲染到文件中。|
| [to_image(page_index, stream)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) |将特定页面渲染到流中。|
| [to_tiff(stream)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) |将整个工作表渲染为 Tiff 图像以进行流式传输。|
| [to_tiff(filename)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) |将整个工作表作为 Tiff 图像呈现到文件中。|
| [to_printer(printer_name)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) |将工作表渲染到打印机|
| [to_printer(printer_name, job_name)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) |将工作表渲染到打印机|
| [to_printer(printer_settings)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) |将工作表渲染到打印机|
| [to_printer(printer_settings, job_name)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) |将工作表渲染到打印机|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) |将工作表渲染到打印机|
| [get_page_size_inch(page_index)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |获取以英寸输出图像为单位的页面大小。|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/zh/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) |使用此功能打印每一页时，客户端可以控制打印机的页面设置。|



### 也可以看看
* 模块 [aspose.cells.rendering](..)
