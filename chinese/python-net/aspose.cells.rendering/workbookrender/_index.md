---
title: WorkbookRender类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 130
url: /zh/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
## WorkbookRender类
代表工作簿渲染。
该类的构造函数，必须在pagesetup、cell style修改后使用。



WorkbookRender 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | WorkbookRender 的构造|


### 特性
|属性|描述|
| :- | :- |
| [page_count](/cells/zh/python-net/aspose.cells.rendering/workbookrender/page_count) |获取工作簿的总页数。|


### 方法
|方法|描述|
| :- | :- |
| [to_image(stream)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) |将整个工作簿渲染为 Tiff Image 以流式传输。|
| [to_image(filename)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_image/#str) |将整个工作簿作为 Tiff 图像呈现到文件中。|
| [to_image(page_index, file_name)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) |将特定页面渲染到文件中。|
| [to_image(page_index, stream)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) |将特定页面渲染到流中。|
| [to_printer(printer_name)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) |将工作簿渲染到打印机|
| [to_printer(printer_name, job_name)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) |将工作簿渲染到打印机|
| [to_printer(printer_settings)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) |将工作簿渲染到打印机|
| [to_printer(printer_settings, job_name)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) |将工作簿渲染到打印机|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) |将工作簿渲染到打印机|
| [get_page_size_inch(page_index)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) |获取以英寸输出图像为单位的页面大小。|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/zh/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) |使用此功能打印每一页时，客户端可以控制打印机的页面设置。|



### 评论



### 也可以看看
* 模块 [aspose.cells.rendering](..)
