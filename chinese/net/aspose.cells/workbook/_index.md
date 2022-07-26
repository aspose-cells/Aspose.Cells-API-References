---
title: Workbook
second_title: Aspose.Cells for .NET API 参考
description: 表示创建 Excel 电子表格的根对象
type: docs
weight: 6480
url: /zh/net/aspose.cells/workbook/
---
## Workbook class

表示创建 Excel 电子表格的根对象。

```csharp
public class Workbook : IDisposable
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [Workbook](workbook#constructor)() | 初始化[`Workbook`](../workbook)类. |
| [Workbook](workbook#constructor_1)(FileFormatType) | 初始化[`Workbook`](../workbook)类. |
| [Workbook](workbook#constructor_2)(Stream) | 初始化[`Workbook`](../workbook)上课并打开一个流。 |
| [Workbook](workbook#constructor_4)(string) | 初始化[`Workbook`](../workbook)上课并打开一个文件。 |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | 初始化[`Workbook`](../workbook)上课并打开流。 |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | 初始化[`Workbook`](../workbook)上课并打开一个文件。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | 获取和设置文件的绝对路径。 |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | 返回一个[`DocumentProperty`](../../aspose.cells.properties/documentproperty)表示电子表格的所有内置文档属性的集合。 |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | 从自定义对象获取用于构建 ICellsDataTable 的工厂 |
| [Colors](../../aspose.cells/workbook/colors) { get; } | 在电子表格的调色板中返回颜色。 |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | 获取列表[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty)工作簿中的对象。 |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | 获取样式池中样式的数量。 |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | 返回一个[`DocumentProperty`](../../aspose.cells.properties/documentproperty)表示电子表格的所有自定义文档属性的集合。 |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | 表示自定义 XML 数据存储部分（包中的自定义 XML 数据）。 |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | 获取[`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection)集合. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | 获取混搭数据。 |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | 获取 DataSorter 对象对数据进行排序。 |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | 获取或设置默认值[`Style`](../style)工作簿的对象. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | 获取和设置文件格式。 |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | 获取并设置当前文件名。 |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | 指示此电子表格是否包含宏/VBA。 |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | 获取工作簿是否有任何跟踪更改 |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | 获取和设置中断监视器。 |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | 指示此电子表格是否经过数字签名。 |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | 表示是否设置了许可证。 |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | 指示结构或窗口是否受密码保护。 |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | 获取和设置定义功能区 UI 的 XML 文件。 |
| [Settings](../../aspose.cells/workbook/settings) { get; } | 表示工作簿设置。 |
| [Theme](../../aspose.cells/workbook/theme) { get; } | 获取主题名称。 |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | 获取[`VbaProject`](./vbaproject)在电子表格中。 |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | 获取[`WorksheetCollection`](../worksheetcollection)电子表格中的集合。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | 接受工作簿中的所有跟踪更改。 |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | 向 OOXML 电子表格文件（Excel2007 及更高版本）添加数字签名。 |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | 计算公式的结果。 |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | 计算公式的结果。 |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | 计算本工作簿中的公式。 |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | 更改指定索引中电子表格的调色板。 |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | 关闭使用缓存访问数据的会话。 |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | 组合另一个工作簿对象。 |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | 从源工作簿对象复制数据。 |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | 从源工作簿对象复制数据。 |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | 从另一个工作簿复制主题。 |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | 按给定类型创建内置样式。 |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | 创建一个[`CellsColor`](../cellscolor)对象. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | 创建新样式。 |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | 自定义主题。 |
| [Dispose](../../aspose.cells/workbook/dispose)() | 执行与释放、释放或 重置非托管资源相关的应用程序定义任务。 |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | 导出 XML 数据。 |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | 导出由指定 XML 映射链接的 XML 数据。 |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | 从文件中获取数字签名。 |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | 获取样式池中的所有字体。 |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | 在当前调色板中找到最佳匹配颜色。 |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | 获取样式池中的命名样式。 |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | 获取样式池中的样式。 将工作簿中的所有样式收集到一个池中。 单元格中只有一个简单的参考索引。 |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | 获取主题颜色。 |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | 将 XML 数据文件导入/更新到工作簿中。 |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | 将 XML 数据文件导入/更新到工作簿中。 |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | 检查颜色是否在电子表格的调色板中。 |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | 解析从模板文件加载或设置为单元格时尚未解析的所有公式。 |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | 保护工作簿。 |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | 保护共享工作簿。 |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | 刷新动态数组公式（根据当前数据溢出到相邻单元格的新范围） |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | 从此电子表格中删除数字签名。 |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | 从此电子表格中删除 VBA/宏。 |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | 删除个人信息。 |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | 删除所有未使用的样式。 |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | 用新数据替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | 用新数据替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | 将单元格的值替换为来自DataTable. |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | 将单元格的值替换为新的双精度值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | 用新整数替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | 用新字符串替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | 用双精度数组替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | 用整数数组替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | 用新字符串替换单元格的值。 |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | 将单元格的值替换为新的字符串数组。 |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | 将工作簿保存到磁盘。 |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | 将工作簿保存到流中。 |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | 将工作簿保存到流中。 |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | 将工作簿保存到磁盘。 |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | 将工作簿保存到磁盘。 |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | 创建结果电子表格并将其传输到客户端，然后在浏览器或 MS Workbook 中打开它。 |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | 创建结果电子表格并将其传输到客户端，然后在浏览器或 MS Workbook 中打开它。 |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | 将 Excel 文件保存到 MemoryStream 对象并返回它。 |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | 将数字签名设置为电子表格文件（Excel2007 及更高版本）。 |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | 设置加密选项。 |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | 设置主题颜色 |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | 启动使用缓存访问数据的会话。 |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | 取消保护工作簿。 |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | 取消保护共享工作簿。 |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | 如果此工作簿包含指向其他数据源的外部链接， Aspose.Cells 将尝试检索最新数据。 |

### 评论

Workbook 类表示 Excel 电子表格。每个电子表格可以包含多个工作表。 该类的基本功能是打开和保存本机excel文件。 该类具有一些高级功能，例如从其他工作簿复制数据，合并两个工作簿和保护Excel电子表格。

### 例子

以下示例从名为designer.xls 的文件加载工作簿，并使工作簿的水平和垂直滚动条不可见。然后，它在电子表格中分别用整数值和字符串值替换两个字符串值，最后将更新后的文件发送到客户端浏览器。

```csharp
[C#]

//打开一个设计器文件
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//设置滚动条
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//用新值替换占位符字符串
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'打开设计器文件
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'设置滚动条
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'用新值替换占位符字符串
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
