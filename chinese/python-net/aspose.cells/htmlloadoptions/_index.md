---
title: HtmlLoadOptions类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 770
url: /zh/python-net/aspose.cells/htmlloadoptions/
is_root: false
---
##  HtmlLoadOptions类
表示导入 html 文件时的选项。



**继承：** [HtmlLoadOptions](/cells/python-net/aspose.cells/htmlloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)



HtmlLoadOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [HtmlLoadOptions()](/cells/zh/python-net/aspose.cells/htmlloadoptions/__init__/#) |创建加载文件的选项。|
| [HtmlLoadOptions(load_format)](/cells/zh/python-net/aspose.cells/htmlloadoptions/__init__/#LoadFormat) |创建加载文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [load_format](/cells/zh/python-net/aspose.cells/htmlloadoptions/load_format) |获取加载格式。|
| [password](/cells/zh/python-net/aspose.cells/htmlloadoptions/password) |获取和设置工作簿的密码。|
| [parsing_formula_on_open](/cells/zh/python-net/aspose.cells/htmlloadoptions/parsing_formula_on_open) |表示读取文件时是否解析公式。|
| [parsing_pivot_cached_records](/cells/zh/python-net/aspose.cells/htmlloadoptions/parsing_pivot_cached_records) |指示加载文件时是否解析枢轴缓存记录。<br/>默认值为假。|
| [language_code](/cells/zh/python-net/aspose.cells/htmlloadoptions/language_code) |获取或设置基于已保存文件的 CountryCode 的 Workbook 版本的用户界面语言。|
| [region](/cells/zh/python-net/aspose.cells/htmlloadoptions/region) |获取或设置加载文件时基于 CountryCode 的系统区域设置。|
| [default_style_settings](/cells/zh/python-net/aspose.cells/htmlloadoptions/default_style_settings) |获取用于初始化工作簿样式的默认样式设置|
| [standard_font](/cells/zh/python-net/aspose.cells/htmlloadoptions/standard_font) |设置默认标准字体名称|
| [standard_font_size](/cells/zh/python-net/aspose.cells/htmlloadoptions/standard_font_size) |设置默认标准字体大小。|
| [interrupt_monitor](/cells/zh/python-net/aspose.cells/htmlloadoptions/interrupt_monitor) |获取和设置中断监视器。|
| [ignore_not_printed](/cells/zh/python-net/aspose.cells/htmlloadoptions/ignore_not_printed) |直接打印文件忽略不打印的数据|
| [check_data_valid](/cells/zh/python-net/aspose.cells/htmlloadoptions/check_data_valid) |检查模板文件中的数据是否有效。|
| [check_excel_restriction](/cells/zh/python-net/aspose.cells/htmlloadoptions/check_excel_restriction) |用户修改单元格相关对象时是否检查excel文件的限制。<br/>例如，excel 不允许输入超过 32K 的字符串值。<br/>当您输入一个大于 32K 的值时，例如 Cell.PutValue(string)，如果此属性为真，您将得到一个异常。<br/>如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后<br/>您可以输出其他文件格式的完整字符串值，例如 CSV。<br/>但是，如果您设置了这种对 excel 文件格式无效的值，<br/>您以后不应将工作簿另存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。|
| [keep_unparsed_data](/cells/zh/python-net/aspose.cells/htmlloadoptions/keep_unparsed_data) |从模板文件加载工作簿时，是否将未解析的数据保留在内存中。默认为真。|
| [load_filter](/cells/zh/python-net/aspose.cells/htmlloadoptions/load_filter) |表示如何加载数据的过滤器。|
| [light_cells_data_handler](/cells/zh/python-net/aspose.cells/htmlloadoptions/light_cells_data_handler) |读取模板文件时处理单元格数据的数据处理器。|
| [memory_setting](/cells/zh/python-net/aspose.cells/htmlloadoptions/memory_setting) |获取或设置内存使用选项。|
| [warning_callback](/cells/zh/python-net/aspose.cells/htmlloadoptions/warning_callback) |获取或设置警告回调。|
| [auto_fitter_options](/cells/zh/python-net/aspose.cells/htmlloadoptions/auto_fitter_options) |获取和设置自动装配选项|
| [auto_filter](/cells/zh/python-net/aspose.cells/htmlloadoptions/auto_filter) |指示加载文件时是否自动过滤数据。|
| [font_configs](/cells/zh/python-net/aspose.cells/htmlloadoptions/font_configs) |获取和设置单独的字体配置。<br/>仅适用于使用此 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions) 加载的 [Workbook](/cells/zh/python-net/aspose.cells/workbook)。|
| [encoding](/cells/zh/python-net/aspose.cells/htmlloadoptions/encoding) |获取和设置默认编码。仅适用于 csv 文件。|
| [load_style_strategy](/cells/zh/python-net/aspose.cells/htmlloadoptions/load_style_strategy) |指示在将字符串值转换为数字或日期时间时对解析值应用样式的策略。|
| [convert_numeric_data](/cells/zh/python-net/aspose.cells/htmlloadoptions/convert_numeric_data) |获取或设置一个值，该值指示文本文件中的字符串是否转换为数字数据。|
| [convert_date_time_data](/cells/zh/python-net/aspose.cells/htmlloadoptions/convert_date_time_data) |获取或设置一个值，该值指示文本文件中的字符串是否转换为日期数据。|
| [keep_precision](/cells/zh/python-net/aspose.cells/htmlloadoptions/keep_precision) |如果长度为 15，则表示是否不解析字符串值。|
| [attached_files_directory](/cells/zh/python-net/aspose.cells/htmlloadoptions/attached_files_directory) |附加文件将保存到的目录。|
| [load_formulas](/cells/zh/python-net/aspose.cells/htmlloadoptions/load_formulas) |表示如果原html文件中有公式，是否导入公式|
| [support_div_tag](/cells/zh/python-net/aspose.cells/htmlloadoptions/support_div_tag) |表示是否支持布局<div>当 html 文件包含时标记<div>标签。默认值为假。|
| [delete_redundant_spaces](/cells/zh/python-net/aspose.cells/htmlloadoptions/delete_redundant_spaces) |指示文本换行时是否删除多余的空格<br>标签。默认值为 false。|
| [auto_fit_cols_and_rows](/cells/zh/python-net/aspose.cells/htmlloadoptions/auto_fit_cols_and_rows) |指示是否自动调整列和行。默认值为假。|
| [convert_formulas_data](/cells/zh/python-net/aspose.cells/htmlloadoptions/convert_formulas_data) |如果为真，当字符串值以字符'='开头时，将字符串转换为公式，默认值为假。|
| [stream_provider](/cells/zh/python-net/aspose.cells/htmlloadoptions/stream_provider) |获取或设置用于导入对象的 StreamProviderImportHtmlFile。|
| [prog_id](/cells/zh/python-net/aspose.cells/htmlloadoptions/prog_id) |获取创建文件的程序ID。<br/>仅适用于 MHT 文件。|


### 方法
|方法|描述|
| :- | :- |
| [set_paper_size(type)](/cells/zh/python-net/aspose.cells/htmlloadoptions/set_paper_size/#PaperSizeType) |从默认打印机设置中设置默认打印纸张尺寸。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [AbstractTextLoadOptions](/cells/zh/python-net/aspose.cells/abstracttextloadoptions)
* 类 [HtmlLoadOptions](/cells/zh/python-net/aspose.cells/htmlloadoptions)
* 类 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
