---
title: TxtLoadOptions类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 1510
url: /zh/python-net/aspose.cells/txtloadoptions/
is_root: false
---
## TxtLoadOptions类
表示加载文本文件的选项。



**继承：** [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) → 
[AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)



TxtLoadOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [TxtLoadOptions()](/cells/zh/python-net/aspose.cells/txtloadoptions/__init__/#) |创建用于加载文本文件的选项。|
| [TxtLoadOptions(load_format)](/cells/zh/python-net/aspose.cells/txtloadoptions/__init__/#LoadFormat) |创建用于加载文本文件的选项。|


### 特性
|属性|描述|
| :- | :- |
| [load_format](/cells/zh/python-net/aspose.cells/txtloadoptions/load_format) |获取加载格式。|
| [password](/cells/zh/python-net/aspose.cells/txtloadoptions/password) |获取和设置工作簿的密码。|
| [parsing_formula_on_open](/cells/zh/python-net/aspose.cells/txtloadoptions/parsing_formula_on_open) |表示读取文件时是否解析公式。|
| [parsing_pivot_cached_records](/cells/zh/python-net/aspose.cells/txtloadoptions/parsing_pivot_cached_records) |指示加载文件时是否解析枢轴缓存记录。<br/>默认值为假。|
| [language_code](/cells/zh/python-net/aspose.cells/txtloadoptions/language_code) |获取或设置基于已保存文件的 CountryCode 的 Workbook 版本的用户界面语言。|
| [region](/cells/zh/python-net/aspose.cells/txtloadoptions/region) |获取或设置加载文件时基于 CountryCode 的系统区域设置。|
| [default_style_settings](/cells/zh/python-net/aspose.cells/txtloadoptions/default_style_settings) |获取用于初始化工作簿样式的默认样式设置|
| [standard_font](/cells/zh/python-net/aspose.cells/txtloadoptions/standard_font) |设置默认标准字体名称|
| [standard_font_size](/cells/zh/python-net/aspose.cells/txtloadoptions/standard_font_size) |设置默认标准字体大小。|
| [interrupt_monitor](/cells/zh/python-net/aspose.cells/txtloadoptions/interrupt_monitor) |获取和设置中断监视器。|
| [ignore_not_printed](/cells/zh/python-net/aspose.cells/txtloadoptions/ignore_not_printed) |直接打印文件忽略不打印的数据|
| [check_data_valid](/cells/zh/python-net/aspose.cells/txtloadoptions/check_data_valid) |检查模板文件中的数据是否有效。|
| [check_excel_restriction](/cells/zh/python-net/aspose.cells/txtloadoptions/check_excel_restriction) |用户修改单元格相关对象时是否检查excel文件的限制。<br/>例如，excel 不允许输入超过 32K 的字符串值。<br/>当您输入一个大于 32K 的值时，例如 Cell.PutValue(string)，如果此属性为真，您将得到一个异常。<br/>如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后<br/>您可以输出其他文件格式的完整字符串值，例如 CSV。<br/>但是，如果您设置了这种对 excel 文件格式无效的值，<br/>您以后不应将工作簿另存为 excel 文件格式。|
| [keep_unparsed_data](/cells/zh/python-net/aspose.cells/txtloadoptions/keep_unparsed_data) |从模板文件加载时是否将未解析的数据保留在内存中，默认为true。|
| [load_filter](/cells/zh/python-net/aspose.cells/txtloadoptions/load_filter) |表示如何加载数据的过滤器。|
| [light_cells_data_handler](/cells/zh/python-net/aspose.cells/txtloadoptions/light_cells_data_handler) |读取模板文件时处理单元格数据的数据处理器。|
| [memory_setting](/cells/zh/python-net/aspose.cells/txtloadoptions/memory_setting) |获取或设置内存使用选项。|
| [warning_callback](/cells/zh/python-net/aspose.cells/txtloadoptions/warning_callback) |获取或设置警告回调。|
| [auto_fitter_options](/cells/zh/python-net/aspose.cells/txtloadoptions/auto_fitter_options) |获取和设置自动装配选项|
| [auto_filter](/cells/zh/python-net/aspose.cells/txtloadoptions/auto_filter) |指示加载文件时是否自动过滤数据。|
| [font_configs](/cells/zh/python-net/aspose.cells/txtloadoptions/font_configs) |获取和设置单独的字体配置。<br/>仅适用于使用此 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions) 加载的 [Workbook](/cells/zh/python-net/aspose.cells/workbook)。|
| [encoding](/cells/zh/python-net/aspose.cells/txtloadoptions/encoding) |获取和设置默认编码。|
| [load_style_strategy](/cells/zh/python-net/aspose.cells/txtloadoptions/load_style_strategy) |指示在将字符串值转换为数字或日期时间时对解析值应用样式的策略。|
| [convert_numeric_data](/cells/zh/python-net/aspose.cells/txtloadoptions/convert_numeric_data) |获取或设置一个值，该值指示文本文件中的字符串是否转换为数字数据。|
| [convert_date_time_data](/cells/zh/python-net/aspose.cells/txtloadoptions/convert_date_time_data) |获取或设置一个值，该值指示文本文件中的字符串是否转换为日期数据。|
| [keep_precision](/cells/zh/python-net/aspose.cells/txtloadoptions/keep_precision) |如果长度为 15，则表示是否不解析字符串值。|
| [separator](/cells/zh/python-net/aspose.cells/txtloadoptions/separator) |获取和设置文本文件的字符分隔符。|
| [separator_string](/cells/zh/python-net/aspose.cells/txtloadoptions/separator_string) |获取和设置一个字符串值作为分隔符。|
| [is_multi_encoded](/cells/zh/python-net/aspose.cells/txtloadoptions/is_multi_encoded) | True 表示文件包含多种编码。|
| [preferred_parsers](/cells/zh/python-net/aspose.cells/txtloadoptions/preferred_parsers) |获取和设置用于加载文本文件的首选值解析器。|
| [has_formula](/cells/zh/python-net/aspose.cells/txtloadoptions/has_formula) |如果文本以“=”开头，则表示文本是否为公式。|
| [has_text_qualifier](/cells/zh/python-net/aspose.cells/txtloadoptions/has_text_qualifier) |是否有单元格值的文本限定符。默认为 true。|
| [text_qualifier](/cells/zh/python-net/aspose.cells/txtloadoptions/text_qualifier) |指定单元格值的文本限定符。默认限定符是“”。|
| [treat_consecutive_delimiters_as_one](/cells/zh/python-net/aspose.cells/txtloadoptions/treat_consecutive_delimiters_as_one) |是否应将连续的定界符视为一个。|
| [treat_quote_prefix_as_value](/cells/zh/python-net/aspose.cells/txtloadoptions/treat_quote_prefix_as_value) |指示前导单引号是否应作为一个单元格值的一部分。<br/>默认为 true。如果为 false，则将从相应单元格的值中删除前导单引号<br/>和 [Style.quote_prefix](/cells/zh/python-net/aspose.cells/style#quote_prefix) 将被设置为真为单元格。|
| [extend_to_next_sheet](/cells/zh/python-net/aspose.cells/txtloadoptions/extend_to_next_sheet) |当数据的行数或列数超过限制时，是否将数据扩展到下一张工作表。<br/>如果此属性为真，则额外数据将扩展到当前工作表后面的下一个工作表（如果当前工作表是最后一个工作表，<br/>新工作表将附加到当前工作簿）。<br/>如果此属性为 false，则忽略超出限制的数据。<br/>默认为假；|


### 方法
|方法|描述|
| :- | :- |
| [set_paper_size(type)](/cells/zh/python-net/aspose.cells/txtloadoptions/set_paper_size/#PaperSizeType) |从默认打印机设置中设置默认打印纸张尺寸。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [AbstractTextLoadOptions](/cells/zh/python-net/aspose.cells/abstracttextloadoptions)
* 类 [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions)
* 类 [TxtLoadOptions](/cells/zh/python-net/aspose.cells/txtloadoptions)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
