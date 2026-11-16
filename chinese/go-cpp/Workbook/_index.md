---
title: "Workbook 类"
linktitle: "Workbook"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Workbook 类。封装在 Go 中表示 workbook 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/workbook/
---

## Workbook class

表示用于创建 Excel 电子表格的根对象。

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewWorkbook](./newworkbook/) | 初始化 Workbook 类的新实例。 |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | 初始化 Workbook 类的新实例。 |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | 使用选项初始化 Workbook 类的一个新的空实例 |
| [NewWorkbook_String](./newworkbook_string/) | 初始化 Workbook 类的新实例并打开文件。 |
| [NewWorkbook_Stream](./newworkbook_stream/) | 初始化 Workbook 类的新实例并打开流。 |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | 初始化 Workbook 类的新实例并打开文件。 |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | 初始化 Workbook 类的新实例并打开流。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSettings](./getsettings/) | 表示工作簿设置。 |
| [ParseFormulas](./parseformulas/) | 解析所有在从模板文件加载或设置到单元格时尚未解析的公式。 |
| [StartAccessCache](./startaccesscache/) | 启动使用缓存访问数据的会话。 |
| [CloseAccessCache](./closeaccesscache/) | 关闭使用缓存访问数据的会话。 |
| [Save_String_SaveFormat](./save_string_saveformat/) | 将工作簿保存到磁盘。 |
| [Save_String](./save_string/) | 保存工作簿到磁盘。 |
| [Save_String_SaveOptions](./save_string_saveoptions/) | 将工作簿保存到磁盘。 |
| [Save_SaveFormat](./save_saveformat/) | 将工作簿保存到流中。 |
| [Save_SaveOptions](./save_saveoptions/) | 将工作簿保存到流中。 |
| [SaveToStream](./savetostream/) | 将 Excel 文件保存到 MemoryStream 对象中，作为 Excel97-2003 xls 文件并返回它。 |
| [GetWorksheets](./getworksheets/) | 获取电子表格中的 WorksheetCollection 集合。 |
| [IsLicensed](./islicensed/) | 指示是否已设置许可证。 |
| [RemoveUnusedStyles](./removeunusedstyles/) | 移除所有未使用的样式。 |
| [CreateStyle](./createstyle/) | 创建新样式。 |
| [CreateStyle_Bool](./createstyle_bool/) | 创建新样式。 |
| [CreateBuiltinStyle](./createbuiltinstyle/) | 根据给定类型创建内置样式。 |
| [CreateCellsColor](./createcellscolor/) | 创建 CellsColor 对象。 |
| [Replace_String_String](./replace_string_string/) | 将单元格的值替换为新的字符串。 |
| [Replace_String_Int](./replace_string_int/) | 将单元格的值替换为新的整数。 |
| [Replace_String_Double](./replace_string_double/) | 将单元格的值替换为新的双精度数。 |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | 将单元格的值替换为新的字符串数组。 |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | 将单元格的值替换为整数数组。 |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | 将单元格的值替换为双精度数组。 |
| [Replace_Bool_Object](./replace_bool_object/) | 将单元格的值替换为新数据。 |
| [Replace_Int_Object](./replace_int_object/) | 将单元格的值替换为新数据。 |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | 将单元格的值替换为新的字符串。 |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | 复制另一个 Workbook 对象。 |
| [Copy_Workbook](./copy_workbook/) | 从源 Workbook 对象复制数据。 |
| [Combine](./combine/) | 合并另一个 Workbook 对象。 |
| [GetColors](./getcolors/) | 返回电子表格调色板中的颜色。 |
| [GetStyleInPool](./getstyleinpool/) | 获取样式池中的样式。工作簿中的所有样式将被收集到池中。单元格中只有一个简单的引用索引。 |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | 获取样式池中样式的数量。 |
| [GetFonts](./getfonts/) | 获取样式池中的所有字体。 |
| [GetNamedStyle](./getnamedstyle/) | 获取样式池中的命名样式。 |
| [MergeNamedStyles](./mergenamedstyles/) | 合并来自其他 Excel 文件的命名样式。 |
| [ChangePalette](./changepalette/) | 更改指定索引处电子表格的调色板。 |
| [IsColorInPalette](./iscolorinpalette/) | 检查颜色是否在电子表格的调色板中。 |
| [CalculateFormula](./calculateformula/) | 计算公式的结果。 |
| [CalculateFormula_Bool](./calculateformula_bool/) | 计算公式的结果。 |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | 正在计算此工作簿中的公式。 |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | 刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围），工作簿中的其他公式即使被动态数组公式使用也不会递归计算。 |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | 刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围）。 |
| [GetDefaultStyle](./getdefaultstyle/) | 获取或设置工作簿的默认 Style 对象。 |
| [SetDefaultStyle](./setdefaultstyle/) | 获取或设置工作簿的默认 Style 对象。 |
| [GetMatchingColor](./getmatchingcolor/) | 在当前调色板中查找最匹配的 Color。 |
| [IsDigitallySigned](./isdigitallysigned/) | 指示此电子表格是否已数字签名。 |
| [SetEncryptionOptions](./setencryptionoptions/) | 设置加密选项。 |
| [Protect](./protect/) | 保护工作簿。 |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | 保护共享工作簿。 |
| [Unprotect](./unprotect/) | 取消保护工作簿。 |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | 取消保护共享工作簿。 |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | 指示结构或窗口是否已使用密码受保护。 |
| [RemoveMacro](./removemacro/) | 从此电子表格中移除 VBA/宏。 |
| [GetVbaProject](./getvbaproject/) | 获取电子表格中的 VbaProject。 |
| [RemoveDigitalSignature](./removedigitalsignature/) | 从此电子表格中移除数字签名。 |
| [AcceptAllRevisions](./acceptallrevisions/) | 接受工作簿中的所有已跟踪更改。 |
| [GetHasMacro](./gethasmacro/) | 指示此电子表格是否包含宏/VBA。 |
| [GetHasRevisions](./gethasrevisions/) | 获取工作簿是否有任何已跟踪更改。 |
| [GetFileName](./getfilename/) | 获取并设置当前文件名。 |
| [SetFileName](./setfilename/) | 获取并设置当前文件名。 |
| [GetDataSorter](./getdatasorter/) | 获取用于排序数据的 DataSorter 对象。 |
| [GetThemeColor](./getthemecolor/) | 获取主题颜色。 |
| [SetThemeColor](./setthemecolor/) | 设置主题颜色 |
| [GetTheme](./gettheme/) | 获取主题名称。 |
| [CustomTheme](./customtheme/) | 自定义主题。 |
| [CopyTheme](./copytheme/) | 从另一本工作簿复制主题。 |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | 更新自定义函数的定义。 |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | 如果此工作簿包含指向其他数据源的外部链接，Aspose.Cells 将尝试从给定来源检索最新数据。 |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有内置文档属性。 |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | 返回一个 DocumentProperty 集合，表示电子表格的所有自定义文档属性。 |
| [GetFileFormat](./getfileformat/) | 获取和设置文件格式。 |
| [SetFileFormat](./setfileformat/) | 获取和设置文件格式。 |
| [GetHasCustomFunction](./gethascustomfunction/) | 检测此工作簿中是否使用了自定义函数，例如在单元格公式、已定义名称中…… |
| [GetInterruptMonitor](./getinterruptmonitor/) | 获取并设置中断监视器。 |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | 获取并设置中断监视器。 |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | 设置中断监视器。 |
| [GetContentTypeProperties](./getcontenttypeproperties/) | 获取工作簿中 ContentTypeProperty 对象的列表。 |
| [GetCustomXmlParts](./getcustomxmlparts/) | 表示自定义 XML 数据存储部件（包内的自定义 XML 数据）。 |
| [GetDataMashup](./getdatamashup/) | 获取 mashup 数据。 |
| [GetRibbonXml](./getribbonxml/) | 获取和设置定义 Ribbon UI 的 XML 文件。 |
| [SetRibbonXml](./setribbonxml/) | 获取和设置定义 Ribbon UI 的 XML 文件。 |
| [GetAbsolutePath](./getabsolutepath/) | 获取和设置文件的绝对路径。 |
| [SetAbsolutePath](./setabsolutepath/) | 获取和设置文件的绝对路径。 |
| [GetDataConnections](./getdataconnections/) | 获取 ExternalConnection 集合。 |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | 导入/更新 XML 数据文件到工作簿中。 |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | 导入/更新 XML 数据文件到工作簿中。 |
| [ExportXml_String_String](./exportxml_string_string/) | 导出由指定 XML 映射链接的 XML 数据。 |
| [ExportXml_String](./exportxml_string/) | 导出 XML 数据。 |
| [SetDigitalSignature](./setdigitalsignature/) | 为电子表格文件（Excel2007 及更高版本）设置数字签名。 |
| [AddDigitalSignature](./adddigitalsignature/) | 向 OOXML 电子表格文件（Excel2007 及更高版本）添加数字签名。 |
| [GetDigitalSignature](./getdigitalsignature/) | 从文件获取数字签名。 |
| [RemovePersonalInformation](./removepersonalinformation/) | 删除个人信息。 |
| [GetDataModel](./getdatamodel/) | 获取工作簿中的数据模型。 |
| [RefreshAll](./refreshall/) | 刷新已链接的形状、所有数据透视表和带有数据透视源的图表。 |
| [Dispose](./dispose/) | 执行应用程序定义的任务，涉及释放、释放或重置非托管资源。 |
