---
title: Workbook类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1590
url: /zh/python-net/aspose.cells/workbook/
is_root: false
---
## Workbook类
表示用于创建 Excel 电子表格的根对象。



Workbook 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [Workbook()](/cells/zh/python-net/aspose.cells/workbook/__init__/#) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例。|
| [Workbook(file_format_type)](/cells/zh/python-net/aspose.cells/workbook/__init__/#FileFormatType) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例。|
| [Workbook(file)](/cells/zh/python-net/aspose.cells/workbook/__init__/#str) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开一个文件。|
| [Workbook(stream)](/cells/zh/python-net/aspose.cells/workbook/__init__/#io.RawIOBase) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开流。|
| [Workbook(file, load_options)](/cells/zh/python-net/aspose.cells/workbook/__init__/#str-LoadOptions) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开一个文件。|
| [Workbook(stream, load_options)](/cells/zh/python-net/aspose.cells/workbook/__init__/#io.RawIOBase-LoadOptions) |初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开流。|


### 特性
|属性|描述|
| :- | :- |
| [settings](/cells/zh/python-net/aspose.cells/workbook/settings) |表示工作簿设置。|
| [worksheets](/cells/zh/python-net/aspose.cells/workbook/worksheets) |获取电子表格中的 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection) 集合。|
| [is_licensed](/cells/zh/python-net/aspose.cells/workbook/is_licensed) |是否设置了license。|
| [colors](/cells/zh/python-net/aspose.cells/workbook/colors) |返回电子表格调色板中的颜色。|
| [count_of_styles_in_pool](/cells/zh/python-net/aspose.cells/workbook/count_of_styles_in_pool) |获取样式池中的样式数。|
| [default_style](/cells/zh/python-net/aspose.cells/workbook/default_style) |获取或设置工作簿的默认 [Style](/cells/zh/python-net/aspose.cells/style) 对象。|
| [is_digitally_signed](/cells/zh/python-net/aspose.cells/workbook/is_digitally_signed) |指示此电子表格是否经过数字签名。|
| [is_workbook_protected_with_password](/cells/zh/python-net/aspose.cells/workbook/is_workbook_protected_with_password) |指示结构或窗口是否受密码保护。|
| [vba_project](/cells/zh/python-net/aspose.cells/workbook/vba_project) |获取电子表格中的 [Workbook.vba_project](/cells/zh/python-net/aspose.cells/workbook#vba_project)。|
| [has_macro](/cells/zh/python-net/aspose.cells/workbook/has_macro) |指示此电子表格是否包含宏/VBA。|
| [has_revisions](/cells/zh/python-net/aspose.cells/workbook/has_revisions) |获取工作簿是否有任何跟踪更改|
| [file_name](/cells/zh/python-net/aspose.cells/workbook/file_name) |获取和设置当前文件名。|
| [cells_data_table_factory](/cells/zh/python-net/aspose.cells/workbook/cells_data_table_factory) |获取用于从自定义对象构建 ICellsDataTable 的工厂|
| [data_sorter](/cells/zh/python-net/aspose.cells/workbook/data_sorter) |获取 DataSorter 对象以对数据进行排序。|
| [theme](/cells/zh/python-net/aspose.cells/workbook/theme) |获取主题名称。|
| [built_in_document_properties](/cells/zh/python-net/aspose.cells/workbook/built_in_document_properties) |返回代表电子表格所有内置文档属性的 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 集合。|
| [custom_document_properties](/cells/zh/python-net/aspose.cells/workbook/custom_document_properties) |返回代表电子表格所有自定义文档属性的 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty) 集合。|
| [file_format](/cells/zh/python-net/aspose.cells/workbook/file_format) |获取和设置文件格式。|
| [interrupt_monitor](/cells/zh/python-net/aspose.cells/workbook/interrupt_monitor) |获取和设置中断监视器。|
| [content_type_properties](/cells/zh/python-net/aspose.cells/workbook/content_type_properties) |获取工作簿中 [ContentTypeProperty](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty) 对象的列表。|
| [custom_xml_parts](/cells/zh/python-net/aspose.cells/workbook/custom_xml_parts) |表示自定义 XML 数据存储部件（包内的自定义 XML 数据）。|
| [data_mashup](/cells/zh/python-net/aspose.cells/workbook/data_mashup) |获取混搭数据。|
| [ribbon_xml](/cells/zh/python-net/aspose.cells/workbook/ribbon_xml) |获取和设置定义功能区 UI 的 XML 文件。|
| [absolute_path](/cells/zh/python-net/aspose.cells/workbook/absolute_path) |获取和设置文件的绝对路径。|
| [data_connections](/cells/zh/python-net/aspose.cells/workbook/data_connections) |获取 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection) 集合。|


### 方法
|方法|描述|
| :- | :- |
| [save(file_name, save_format)](/cells/zh/python-net/aspose.cells/workbook/save/#str-SaveFormat) |将工作簿保存到磁盘。|
| [save(file_name)](/cells/zh/python-net/aspose.cells/workbook/save/#str) |将工作簿保存到磁盘。|
| [save(file_name, save_options)](/cells/zh/python-net/aspose.cells/workbook/save/#str-SaveOptions) |将工作簿保存到磁盘。|
| [save(stream, save_format)](/cells/zh/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveFormat) |将工作簿保存到流中。|
| [save(stream, save_options)](/cells/zh/python-net/aspose.cells/workbook/save/#io.RawIOBase-SaveOptions) |将工作簿保存到流中。|
| [replace(place_holder, new_value)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-str) |用新字符串替换单元格的值。|
| [replace(place_holder, new_value)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-int) |用新整数替换单元格的值。|
| [replace(place_holder, new_value)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-float) |用新的双精度替换单元格的值。|
| [replace(place_holder, new_values, is_vertical)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-list-bool) |用新的字符串数组替换单元格的值。|
| [replace(place_holder, new_values, is_vertical)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-list-bool) |用整数数组替换单元格的值。|
| [replace(place_holder, new_values, is_vertical)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-list-bool) |用双精度数组替换单元格的值。|
| [replace(bool_value, new_value)](/cells/zh/python-net/aspose.cells/workbook/replace/#bool-any) |用新数据替换单元格的值。|
| [replace(int_value, new_value)](/cells/zh/python-net/aspose.cells/workbook/replace/#int-any) |用新数据替换单元格的值。|
| [replace(place_holder, new_value, options)](/cells/zh/python-net/aspose.cells/workbook/replace/#str-str-ReplaceOptions) |用新字符串替换单元格的值。|
| [copy(source, copy_options)](/cells/zh/python-net/aspose.cells/workbook/copy/#Workbook-CopyOptions) |从源工作簿对象复制数据。|
| [copy(source)](/cells/zh/python-net/aspose.cells/workbook/copy/#Workbook) |从源工作簿对象复制数据。|
| [calculate_formula()](/cells/zh/python-net/aspose.cells/workbook/calculate_formula/#) |计算公式的结果。|
| [calculate_formula(ignore_error)](/cells/zh/python-net/aspose.cells/workbook/calculate_formula/#bool) |计算公式的结果。|
| [calculate_formula(ignore_error, custom_function)](/cells/zh/python-net/aspose.cells/workbook/calculate_formula/#bool-ICustomFunction) |计算公式的结果。|
| [calculate_formula(options)](/cells/zh/python-net/aspose.cells/workbook/calculate_formula/#CalculationOptions) |计算本工作簿中的公式。|
| [refresh_dynamic_array_formulas(calculate)](/cells/zh/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool) |刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围）<br/>工作簿中的其他公式即使被动态数组公式使用也不会递归计算。|
| [refresh_dynamic_array_formulas(calculate, copts)](/cells/zh/python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/#bool-CalculationOptions) |刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围）|
| [import_xml(url, sheet_name, row, col)](/cells/zh/python-net/aspose.cells/workbook/import_xml/#str-str-int-int) |将 XML 数据文件导入/更新到工作簿中。|
| [import_xml(stream, sheet_name, row, col)](/cells/zh/python-net/aspose.cells/workbook/import_xml/#io.RawIOBase-str-int-int) |将 XML 数据文件导入/更新到工作簿中。|
| [export_xml(map_name, path)](/cells/zh/python-net/aspose.cells/workbook/export_xml/#str-str) |导出由指定 XML 映射链接的 XML 数据。|
| [export_xml(map_name, stream)](/cells/zh/python-net/aspose.cells/workbook/export_xml/#str-io.RawIOBase) |导出 XML 数据。|
| [parse_formulas(ignore_error)](/cells/zh/python-net/aspose.cells/workbook/parse_formulas/#bool) |解析所有从模板文件加载或设置到单元格时尚未解析的公式。|
| [start_access_cache(opts)](/cells/zh/python-net/aspose.cells/workbook/start_access_cache/#AccessCacheOptions) |启动使用缓存访问数据的会话。|
| [close_access_cache(opts)](/cells/zh/python-net/aspose.cells/workbook/close_access_cache/#AccessCacheOptions) |关闭使用缓存访问数据的会话。|
| [remove_unused_styles()](/cells/zh/python-net/aspose.cells/workbook/remove_unused_styles/#) |删除所有未使用的样式。|
| [create_style()](/cells/zh/python-net/aspose.cells/workbook/create_style/#) |创建一个新的样式。|
| [create_builtin_style(type)](/cells/zh/python-net/aspose.cells/workbook/create_builtin_style/#BuiltinStyleType) |按给定类型创建内置样式。|
| [create_cells_color()](/cells/zh/python-net/aspose.cells/workbook/create_cells_color/#) |创建一个 [CellsColor](/cells/zh/python-net/aspose.cells/cellscolor) 对象。|
| [combine(second_workbook)](/cells/zh/python-net/aspose.cells/workbook/combine/#Workbook) |合并另一个 Workbook 对象。|
| [get_style_in_pool(index)](/cells/zh/python-net/aspose.cells/workbook/get_style_in_pool/#int) |获取样式池中的样式。<br/>工作簿中的所有样式都将汇集到一个池中。<br/>单元格中只有一个简单的参考索引。|
| [get_fonts()](/cells/zh/python-net/aspose.cells/workbook/get_fonts/#) |获取样式池中的所有字体。|
| [get_named_style(name)](/cells/zh/python-net/aspose.cells/workbook/get_named_style/#str) |获取样式池中的命名样式。|
| [change_palette(color, index)](/cells/zh/python-net/aspose.cells/workbook/change_palette/#aspose.pydrawing.Color-int) |更改指定索引中电子表格的调色板。|
| [is_color_in_palette(color)](/cells/zh/python-net/aspose.cells/workbook/is_color_in_palette/#aspose.pydrawing.Color) |检查颜色是否在电子表格的调色板中。|
| [get_matching_color(raw_color)](/cells/zh/python-net/aspose.cells/workbook/get_matching_color/#aspose.pydrawing.Color) |在当前调色板中找到最匹配的颜色。|
| [set_encryption_options(encryption_type, key_length)](/cells/zh/python-net/aspose.cells/workbook/set_encryption_options/#EncryptionType-int) |设置加密选项。|
| [protect(protection_type, password)](/cells/zh/python-net/aspose.cells/workbook/protect/#ProtectionType-str) |保护工作簿。|
| [protect_shared_workbook(password)](/cells/zh/python-net/aspose.cells/workbook/protect_shared_workbook/#str) |保护共享工作簿。|
| [unprotect(password)](/cells/zh/python-net/aspose.cells/workbook/unprotect/#str) |取消保护工作簿。|
| [unprotect_shared_workbook(password)](/cells/zh/python-net/aspose.cells/workbook/unprotect_shared_workbook/#str) |取消保护共享工作簿。|
| [remove_macro()](/cells/zh/python-net/aspose.cells/workbook/remove_macro/#) |从此电子表格中删除 VBA/宏。|
| [remove_digital_signature()](/cells/zh/python-net/aspose.cells/workbook/remove_digital_signature/#) |从此电子表格中删除数字签名。|
| [accept_all_revisions()](/cells/zh/python-net/aspose.cells/workbook/accept_all_revisions/#) |接受工作簿中的所有修订。|
| [remove_external_links()](/cells/zh/python-net/aspose.cells/workbook/remove_external_links/#) |删除工作簿中的所有外部链接。|
| [get_theme_color(type)](/cells/zh/python-net/aspose.cells/workbook/get_theme_color/#ThemeColorType) |获取主题颜色。|
| [set_theme_color(type, color)](/cells/zh/python-net/aspose.cells/workbook/set_theme_color/#ThemeColorType-aspose.pydrawing.Color) |设置主题颜色|
| [custom_theme(theme_name, colors)](/cells/zh/python-net/aspose.cells/workbook/custom_theme/#str-aspose.pydrawing.Color[]) |海关主题。|
| [copy_theme(source)](/cells/zh/python-net/aspose.cells/workbook/copy_theme/#Workbook) |从另一个工作簿复制主题。|
| [has_exernal_links()](/cells/zh/python-net/aspose.cells/workbook/has_exernal_links/#) |指示此工作簿是否包含指向其他数据源的外部链接。|
| [update_linked_data_source(external_workbooks)](/cells/zh/python-net/aspose.cells/workbook/update_linked_data_source/#list) |如果此工作簿包含指向其他数据源的外部链接，<br/> Aspose.Cells 将尝试检索最新数据。|
| [set_digital_signature(digital_signature_collection)](/cells/zh/python-net/aspose.cells/workbook/set_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) |将数字签名设置为电子表格文件（Excel2007 及更高版本）。|
| [add_digital_signature(digital_signature_collection)](/cells/zh/python-net/aspose.cells/workbook/add_digital_signature/#aspose.cells.digitalsignatures.DigitalSignatureCollection) |向 OOXML 电子表格文件（Excel2007 及更高版本）添加数字签名。|
| [get_digital_signature()](/cells/zh/python-net/aspose.cells/workbook/get_digital_signature/#) |从文件中获取数字签名。|
| [remove_personal_information()](/cells/zh/python-net/aspose.cells/workbook/remove_personal_information/#) |删除个人信息。|



### 评论

Workbook 类表示 Excel 电子表格。每个电子表格可以包含多个工作表。
该类的基本功能是打开和保存本机 excel 文件。
该类具有一些高级功能，如从其他工作簿复制数据、合并两个工作簿和保护 Excel 电子表格。

### 例子

以下示例从名为 designer.xls 的文件中加载 Workbook，并使 Workbook 的水平和垂直滚动条不可见。然后在电子表格中分别用整数值和字符串值替换两个字符串值，最后将更新后的文件发送到客户端浏览器。

```python
from aspose.cells import Workbook

# Open a designer file
designerFile = "designer.xls"
workbook = Workbook(designerFile)
# Set scroll bars
workbook.settings.is_h_scroll_bar_visible = False
workbook.settings.is_v_scroll_bar_visible = False
# Replace the placeholder string with new values
newInt = 100
workbook.replace("OldInt", newInt)
newString = "Hello!"
workbook.replace("OldString", newString)
workbook.save("result.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CellsColor](/cells/zh/python-net/aspose.cells/cellscolor)
* 类 [ContentTypeProperty](/cells/zh/python-net/aspose.cells.properties/contenttypeproperty)
* 类 [DocumentProperty](/cells/zh/python-net/aspose.cells.properties/documentproperty)
* 类 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)
* 类 [Style](/cells/zh/python-net/aspose.cells/style)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
* 类 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection)
