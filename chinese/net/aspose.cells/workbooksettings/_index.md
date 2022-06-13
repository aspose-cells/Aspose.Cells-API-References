---
title: WorkbookSettings
second_title: Aspose.Cells for .NET API 参考
description: 代表工作簿的所有设置
type: docs
weight: 6500
url: /zh/net/aspose.cells/workbooksettings/
---
## WorkbookSettings class

代表工作簿的所有设置。

```csharp
public class WorkbookSettings : IDisposable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Author](../../aspose.cells/workbooksettings/author) { get; set; } | 获取和设置文件的作者。 |
| [AutoCompressPictures](../../aspose.cells/workbooksettings/autocompresspictures) { get; set; } | 指定一个布尔值，指示应用程序自动压缩工作簿中的图片。 |
| [AutoRecover](../../aspose.cells/workbooksettings/autorecover) { get; set; } | 指示文件是否标记为自动恢复。 |
| [BuildVersion](../../aspose.cells/workbooksettings/buildversion) { get; set; } | 指定应用程序的增量公开发布。 |
| [CheckCompatibility](../../aspose.cells/workbooksettings/checkcompatibility) { get; set; } | 表示保存工作簿时是否检查与早期版本的兼容性。 |
| [CheckCustomNumberFormat](../../aspose.cells/workbooksettings/checkcustomnumberformat) { get; set; } | 表示设置 Style.Custom 时是否检查自定义数字格式。 |
| [CheckExcelRestriction](../../aspose.cells/workbooksettings/checkexcelrestriction) { get; set; } | 用户修改单元格相关对象时是否检查excel文件的限制。 例如，excel不允许输入超过32K的字符串值。 当你输入一个超过 32K 的值时，比如通过 Cell.PutValue(string)，如果这个属性为真，你会得到一个 Exception。 如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便稍后 您可以为其他文件格式（例如 CSV）输出完整的字符串值。 但是，如果您设置了这种对 excel 文件格式无效的值，则 以后不应将工作簿保存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。 |
| [Compliance](../../aspose.cells/workbooksettings/compliance) { get; set; } | 指定输出文档的 OOXML 版本。默认值为 Ecma376_2006。 |
| [CrashSave](../../aspose.cells/workbooksettings/crashsave) { get; set; } | 指示应用程序是否在崩溃后上次保存工作簿文件。 |
| [CultureInfo](../../aspose.cells/workbooksettings/cultureinfo) { get; set; } | 获取或设置系统文化信息。 |
| [DataExtractLoad](../../aspose.cells/workbooksettings/dataextractload) { get; set; } | 表示应用程序是否上次打开工作簿进行数据恢复。 |
| [Date1904](../../aspose.cells/workbooksettings/date1904) { get; set; } | 获取或设置一个值，该值表示工作簿是否使用 1904 日期系统。 |
| [DisplayDrawingObjects](../../aspose.cells/workbooksettings/displaydrawingobjects) { get; set; } | 指示是否以及如何显示工作簿中的对象。 |
| [EnableMacros](../../aspose.cells/workbooksettings/enablemacros) { get; set; } | 启用宏； |
| [FirstVisibleTab](../../aspose.cells/workbooksettings/firstvisibletab) { get; set; } | 获取或设置第一个可见的工作表选项卡。 |
| [FormulaSettings](../../aspose.cells/workbooksettings/formulasettings) { get; } | 获取公式相关功能的设置。 |
| [GlobalizationSettings](../../aspose.cells/workbooksettings/globalizationsettings) { get; set; } | 获取和设置全球化设置。 |
| [HidePivotFieldList](../../aspose.cells/workbooksettings/hidepivotfieldlist) { get; set; } | 获取并设置是否隐藏数据透视表的字段列表。 |
| [IsDefaultEncrypted](../../aspose.cells/workbooksettings/isdefaultencrypted) { get; set; } | 如果工作簿的结构和窗口被锁定，是否使用默认密码加密工作簿。 |
| [IsEncrypted](../../aspose.cells/workbooksettings/isencrypted) { get; } | 获取一个值，该值指示打开此工作簿是否需要密码。 |
| [IsHidden](../../aspose.cells/workbooksettings/ishidden) { get; set; } | 指示此工作簿是否隐藏。 |
| [IsHScrollBarVisible](../../aspose.cells/workbooksettings/ishscrollbarvisible) { get; set; } | 获取或设置一个值，指示生成的电子表格是否包含水平滚动条。 |
| [IsMinimized](../../aspose.cells/workbooksettings/isminimized) { get; set; } | 表示生成的电子表格是否会被最小化打开。 |
| [IsProtected](../../aspose.cells/workbooksettings/isprotected) { get; } | 获取一个值，该值指示工作簿的结构或窗口是否受到保护。 |
| [IsVScrollBarVisible](../../aspose.cells/workbooksettings/isvscrollbarvisible) { get; set; } | 获取或设置一个值，指示生成的电子表格是否包含垂直滚动条。 |
| [LanguageCode](../../aspose.cells/workbooksettings/languagecode) { get; set; } | 根据保存文件的 CountryCode 获取或设置 Workbook 版本的用户界面语言。 |
| [MaxColumn](../../aspose.cells/workbooksettings/maxcolumn) { get; } | 获取最大列索引，从零开始。 |
| [MaxRow](../../aspose.cells/workbooksettings/maxrow) { get; } | 获取最大行索引，从零开始。 |
| [MaxRowsOfSharedFormula](../../aspose.cells/workbooksettings/maxrowsofsharedformula) { get; set; } | 获取和设置共享公式的最大行数。 |
| [MemorySetting](../../aspose.cells/workbooksettings/memorysetting) { get; set; } | 获取或设置内存使用选项。新选项将作为新创建的工作表的默认选项，但不会对现有工作表生效。 |
| [NumberDecimalSeparator](../../aspose.cells/workbooksettings/numberdecimalseparator) { get; set; } | 获取或设置用于格式化/解析数值的小数分隔符。默认为当前 Region 的小数点分隔符。 |
| [NumberGroupSeparator](../../aspose.cells/workbooksettings/numbergroupseparator) { get; set; } | 获取或设置用于分隔数值中小数点左侧数字组的字符。默认为当前 Region 的组分隔符。 |
| [PaperSize](../../aspose.cells/workbooksettings/papersize) { get; set; } | 获取和设置默认打印纸尺寸。 |
| [Password](../../aspose.cells/workbooksettings/password) { get; set; } | 代表工作簿文件加密密码。 |
| [ProtectionType](../../aspose.cells/workbooksettings/protectiontype) { get; } | 获取工作簿的保护类型。 |
| [QuotePrefixToStyle](../../aspose.cells/workbooksettings/quoteprefixtostyle) { get; set; } | 表示输入字符串值（以单引号开头）时是否设置[`QuotePrefix`](../style/quoteprefix)属性为单元格 |
| [Region](../../aspose.cells/workbooksettings/region) { get; set; } | 获取或设置工作簿的区域设置。 |
| [RemovePersonalInformation](../../aspose.cells/workbooksettings/removepersonalinformation) { get; set; } | 如果可以从指定的工作簿中删除个人信息，则为真。 |
| [RepairLoad](../../aspose.cells/workbooksettings/repairload) { get; set; } | 指示应用程序上次是在安全模式还是修复模式下打开工作簿。 |
| [ResourceProvider](../../aspose.cells/workbooksettings/resourceprovider) { get; set; } | 获取和设置外部资源的流提供程序，例如为“LinkToFile”类型的图片加载图像数据。 |
| [Shared](../../aspose.cells/workbooksettings/shared) { get; set; } | 获取或设置一个指示工作簿是否共享的值。 |
| [SheetTabBarWidth](../../aspose.cells/workbooksettings/sheettabbarwidth) { get; set; } | 工作表标签栏的宽度（窗口宽度的 1/1000）。 |
| [ShowTabs](../../aspose.cells/workbooksettings/showtabs) { get; set; } | 获取或设置一个值是否显示工作簿选项卡。 |
| [SignificantDigits](../../aspose.cells/workbooksettings/significantdigits) { get; set; } | 获取和设置有效位数。 默认值为[`SignificantDigits`](../cellshelper/significantdigits)。 |
| [UpdateAdjacentCellsBorder](../../aspose.cells/workbooksettings/updateadjacentcellsborder) { get; set; } | 表示是否更新相邻单元格的边框。 |
| [UpdateLinksType](../../aspose.cells/workbooksettings/updatelinkstype) { get; set; } | 获取和设置打开工作簿时如何更新外部链接。 |
| [WarningCallback](../../aspose.cells/workbooksettings/warningcallback) { get; set; } | 获取或设置警告回调。 |
| [WindowHeight](../../aspose.cells/workbooksettings/windowheight) { get; set; } | 窗口的高度，以磅为单位。 |
| [WindowHeightCM](../../aspose.cells/workbooksettings/windowheightcm) { get; set; } | 窗口高度，单位为厘米。 |
| [WindowHeightInch](../../aspose.cells/workbooksettings/windowheightinch) { get; set; } | 窗口高度，单位英寸。 |
| [WindowLeft](../../aspose.cells/workbooksettings/windowleft) { get; set; } | 客户区左边缘到窗口左边缘的距离，以点为单位。 |
| [WindowLeftCM](../../aspose.cells/workbooksettings/windowleftcm) { get; set; } | 客户区左边缘到窗口左边缘的距离。 以厘米为单位。 |
| [WindowLeftInch](../../aspose.cells/workbooksettings/windowleftinch) { get; set; } | 客户区左边缘到窗口左边缘的距离。 以英寸为单位。 |
| [WindowTop](../../aspose.cells/workbooksettings/windowtop) { get; set; } | 客户区上边缘到窗口上边缘的距离，以点为单位。 |
| [WindowTopCM](../../aspose.cells/workbooksettings/windowtopcm) { get; set; } | 客户区上边缘到窗口上边缘的距离，单位为厘米。 |
| [WindowTopInch](../../aspose.cells/workbooksettings/windowtopinch) { get; set; } | 客户区上边缘到窗口上边缘的距离，单位英寸。 |
| [WindowWidth](../../aspose.cells/workbooksettings/windowwidth) { get; set; } | 窗口的宽度，以磅为单位。 |
| [WindowWidthCM](../../aspose.cells/workbooksettings/windowwidthcm) { get; set; } | 窗口的宽度，单位为厘米。 |
| [WindowWidthInch](../../aspose.cells/workbooksettings/windowwidthinch) { get; set; } | 窗口的宽度，单位英寸。 |
| [WriteProtection](../../aspose.cells/workbooksettings/writeprotection) { get; } | 提供对工作簿写保护选项的访问。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Dispose](../../aspose.cells/workbooksettings/dispose)() | 释放资源。 |
| [GetThemeFont](../../aspose.cells/workbooksettings/getthemefont)(FontSchemeType) | 获取默认主题字体名称。 |
| [SetPageOrientationType](../../aspose.cells/workbooksettings/setpageorientationtype)(PageOrientationType) | 设置整个工作簿的打印方向类型。 |

### 例子

```csharp
[C#]

Workbook workbook = new Workbook();

WorkbookSettings settings = workbook.Settings;

 //做你的事

[Visual Basic]
Dim workbook as Workbook = new Workbook()

Dim settings as WorkbookSettings = workbook.Settings

'do your business
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
