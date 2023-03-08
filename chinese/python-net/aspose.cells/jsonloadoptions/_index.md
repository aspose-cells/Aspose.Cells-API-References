---
title: JsonLoadOptions类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 960
url: /zh/python-net/aspose.cells/jsonloadoptions/
is_root: false
---
##  JsonLoadOptions类
代表加载json文件的选项



**继承：** [JsonLoadOptions](/cells/python-net/aspose.cells/jsonloadoptions) → 
[LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)



JsonLoadOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [JsonLoadOptions()](/cells/zh/python-net/aspose.cells/jsonloadoptions/__init__/#) |创建加载文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [load_format](/cells/zh/python-net/aspose.cells/jsonloadoptions/load_format) |获取加载格式。|
| [password](/cells/zh/python-net/aspose.cells/jsonloadoptions/password) |获取和设置工作簿的密码。|
| [parsing_formula_on_open](/cells/zh/python-net/aspose.cells/jsonloadoptions/parsing_formula_on_open) |表示读取文件时是否解析公式。|
| [parsing_pivot_cached_records](/cells/zh/python-net/aspose.cells/jsonloadoptions/parsing_pivot_cached_records) |指示加载文件时是否解析枢轴缓存记录。<br/>默认值为假。|
| [language_code](/cells/zh/python-net/aspose.cells/jsonloadoptions/language_code) |获取或设置基于已保存文件的 CountryCode 的 Workbook 版本的用户界面语言。|
| [region](/cells/zh/python-net/aspose.cells/jsonloadoptions/region) |获取或设置加载文件时基于 CountryCode 的系统区域设置。|
| [default_style_settings](/cells/zh/python-net/aspose.cells/jsonloadoptions/default_style_settings) |获取用于初始化工作簿样式的默认样式设置|
| [standard_font](/cells/zh/python-net/aspose.cells/jsonloadoptions/standard_font) |设置默认标准字体名称|
| [standard_font_size](/cells/zh/python-net/aspose.cells/jsonloadoptions/standard_font_size) |设置默认标准字体大小。|
| [interrupt_monitor](/cells/zh/python-net/aspose.cells/jsonloadoptions/interrupt_monitor) |获取和设置中断监视器。|
| [ignore_not_printed](/cells/zh/python-net/aspose.cells/jsonloadoptions/ignore_not_printed) |直接打印文件忽略不打印的数据|
| [check_data_valid](/cells/zh/python-net/aspose.cells/jsonloadoptions/check_data_valid) |检查模板文件中的数据是否有效。|
| [check_excel_restriction](/cells/zh/python-net/aspose.cells/jsonloadoptions/check_excel_restriction) |用户修改单元格相关对象时是否检查excel文件的限制。<br/>例如，excel 不允许输入超过 32K 的字符串值。<br/>当您输入一个大于 32K 的值时，例如 Cell.PutValue(string)，如果此属性为真，您将得到一个异常。<br/>如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后<br/>您可以输出其他文件格式的完整字符串值，例如 CSV。<br/>但是，如果您设置了这种对 excel 文件格式无效的值，<br/>您以后不应将工作簿另存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。|
| [keep_unparsed_data](/cells/zh/python-net/aspose.cells/jsonloadoptions/keep_unparsed_data) |从模板文件加载工作簿时，是否将未解析的数据保留在内存中。默认为真。|
| [load_filter](/cells/zh/python-net/aspose.cells/jsonloadoptions/load_filter) |表示如何加载数据的过滤器。|
| [light_cells_data_handler](/cells/zh/python-net/aspose.cells/jsonloadoptions/light_cells_data_handler) |读取模板文件时处理单元格数据的数据处理器。|
| [memory_setting](/cells/zh/python-net/aspose.cells/jsonloadoptions/memory_setting) |获取或设置内存使用选项。|
| [warning_callback](/cells/zh/python-net/aspose.cells/jsonloadoptions/warning_callback) |获取或设置警告回调。|
| [auto_fitter_options](/cells/zh/python-net/aspose.cells/jsonloadoptions/auto_fitter_options) |获取和设置自动装配选项|
| [auto_filter](/cells/zh/python-net/aspose.cells/jsonloadoptions/auto_filter) |指示加载文件时是否自动过滤数据。|
| [font_configs](/cells/zh/python-net/aspose.cells/jsonloadoptions/font_configs) |获取和设置单独的字体配置。<br/>仅适用于使用此 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions) 加载的 [Workbook](/cells/zh/python-net/aspose.cells/workbook)。|
| [start_cell](/cells/zh/python-net/aspose.cells/jsonloadoptions/start_cell) |获取和设置起始单元格。|
| [layout_options](/cells/zh/python-net/aspose.cells/jsonloadoptions/layout_options) |导入 json 的选项。|
| [multiple_worksheets](/cells/zh/python-net/aspose.cells/jsonloadoptions/multiple_worksheets) |表示当所有子节点都是数组节点时，是否将JsonObject对象的每个属性作为一个工作表导入。|


### 方法
|方法|描述|
| :- | :- |
| [set_paper_size(type)](/cells/zh/python-net/aspose.cells/jsonloadoptions/set_paper_size/#PaperSizeType) |从默认打印机设置中设置默认打印纸张尺寸。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [JsonLoadOptions](/cells/zh/python-net/aspose.cells/jsonloadoptions)
* 类 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
