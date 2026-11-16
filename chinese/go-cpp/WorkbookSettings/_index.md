---
title: "WorkbookSettings 类"
linktitle: "WorkbookSettings"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "WorkbookSettings 类。封装在 Go 中表示 workbooksettings 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/workbooksettings/
---

## WorkbookSettings class

表示工作簿的所有设置。

```go

type WorkbookSettings struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Dispose](./dispose/) | 释放资源。 |
| [GetThemeFont](./getthemefont/) | 获取默认主题字体名称。 |
| [GetAuthor](./getauthor/) | 获取并设置文件的作者。 |
| [SetAuthor](./setauthor/) | 获取并设置文件的作者。 |
| [GetCheckCustomNumberFormat](./getcheckcustomnumberformat/) | 指示在设置 Style.Custom 时是否检查自定义数字格式。 |
| [SetCheckCustomNumberFormat](./setcheckcustomnumberformat/) | 指示在设置 Style.Custom 时是否检查自定义数字格式。 |
| [GetEnableMacros](./getenablemacros/) | 启用宏； |
| [SetEnableMacros](./setenablemacros/) | 启用宏； |
| [GetDate1904](./getdate1904/) | 获取或设置一个值，表示工作簿是否使用 1904 日期系统。 |
| [SetDate1904](./setdate1904/) | 获取或设置一个值，表示工作簿是否使用 1904 日期系统。 |
| [GetProtectionType](./getprotectiontype/) | 获取工作簿的保护类型。 |
| [GetDisplayDrawingObjects](./getdisplaydrawingobjects/) | 指示是否以及如何在工作簿中显示对象。 |
| [SetDisplayDrawingObjects](./setdisplaydrawingobjects/) | 指示是否以及如何在工作簿中显示对象。 |
| [GetSheetTabBarWidth](./getsheettabbarwidth/) | 工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。 |
| [SetSheetTabBarWidth](./setsheettabbarwidth/) | 工作表选项卡栏的宽度（以窗口宽度的千分之一为单位）。 |
| [GetShowTabs](./getshowtabs/) | 获取或设置一个值，指示是否显示工作簿选项卡。 |
| [SetShowTabs](./setshowtabs/) | 获取或设置一个值，指示是否显示工作簿选项卡。 |
| [GetFirstVisibleTab](./getfirstvisibletab/) | 获取或设置第一个可见的工作表选项卡。 |
| [SetFirstVisibleTab](./setfirstvisibletab/) | 获取或设置第一个可见的工作表选项卡。 |
| [IsHScrollBarVisible](./ishscrollbarvisible/) | 获取或设置一个值，指示生成的电子表格是否包含水平滚动条。 |
| [SetIsHScrollBarVisible](./setishscrollbarvisible/) | 获取或设置一个值，指示生成的电子表格是否包含水平滚动条。 |
| [IsVScrollBarVisible](./isvscrollbarvisible/) | 获取或设置一个值，指示生成的电子表格是否包含垂直滚动条。 |
| [SetIsVScrollBarVisible](./setisvscrollbarvisible/) | 获取或设置一个值，指示生成的电子表格是否包含垂直滚动条。 |
| [GetShared](./getshared/) | 获取或设置一个值，指示工作簿是否为共享状态。 |
| [SetShared](./setshared/) | 获取或设置一个值，指示工作簿是否为共享状态。 |
| [GetLanguageCode](./getlanguagecode/) | 获取或设置基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [SetLanguageCode](./setlanguagecode/) | 获取或设置基于已保存文件的 CountryCode 的工作簿版本的用户界面语言。 |
| [GetRegion](./getregion/) | 获取或设置工作簿的区域设置。 |
| [SetRegion](./setregion/) | 获取或设置工作簿的区域设置。 |
| [GetGlobalizationSettings](./getglobalizationsettings/) | 获取并设置全局化设置。 |
| [SetGlobalizationSettings](./setglobalizationsettings/) | 获取并设置全局化设置。 |
| [GetNumberDecimalSeparator](./getnumberdecimalseparator/) | 获取或设置用于格式化/解析数值的十进制分隔符。默认是当前地区的十进制分隔符。 |
| [SetNumberDecimalSeparator](./setnumberdecimalseparator/) | 获取或设置用于格式化/解析数值的十进制分隔符。默认是当前地区的十进制分隔符。 |
| [GetNumberGroupSeparator](./getnumbergroupseparator/) | 获取或设置数值中小数点左侧用于分隔数字组的字符。默认是当前地区的分组分隔符。 |
| [SetNumberGroupSeparator](./setnumbergroupseparator/) | 获取或设置数值中小数点左侧用于分隔数字组的字符。默认是当前地区的分组分隔符。 |
| [GetPassword](./getpassword/) | 表示工作簿文件加密密码。 |
| [SetPassword](./setpassword/) | 表示工作簿文件加密密码。 |
| [GetWriteProtection](./getwriteprotection/) | 提供对工作簿写保护选项的访问。 |
| [IsEncrypted](./isencrypted/) | 获取一个值，指示是否需要密码才能打开此工作簿。 |
| [IsProtected](./isprotected/) | 获取一个值，指示工作簿的结构或窗口是否受保护。 |
| [IsDefaultEncrypted](./isdefaultencrypted/) | 指示当工作簿的结构和窗口被锁定时，是否使用默认密码加密工作簿。 |
| [SetIsDefaultEncrypted](./setisdefaultencrypted/) | 指示当工作簿的结构和窗口被锁定时，是否使用默认密码加密工作簿。 |
| [IsMinimized](./isminimized/) | 表示生成的电子表格是否将以最小化方式打开。 |
| [SetIsMinimized](./setisminimized/) | 表示生成的电子表格是否将以最小化方式打开。 |
| [IsHidden](./ishidden/) | 指示此工作簿是否被隐藏。 |
| [SetIsHidden](./setishidden/) | 指示此工作簿是否被隐藏。 |
| [GetAutoCompressPictures](./getautocompresspictures/) | 指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。 |
| [SetAutoCompressPictures](./setautocompresspictures/) | 指定一个布尔值，指示应用程序是否自动压缩工作簿中的图片。 |
| [GetRemovePersonalInformation](./getremovepersonalinformation/) | 如果可以从指定的工作簿中删除个人信息，则为 True。 |
| [SetRemovePersonalInformation](./setremovepersonalinformation/) | 如果可以从指定的工作簿中删除个人信息，则为 True。 |
| [GetShapeDisplayType](./getshapedisplaytype/) | 获取和设置应用程序在此工作簿中显示形状的方式 |
| [SetShapeDisplayType](./setshapedisplaytype/) | 获取和设置应用程序在此工作簿中显示形状的方式 |
| [GetHidePivotFieldList](./gethidepivotfieldlist/) | 获取和设置是否隐藏透视表的字段列表。 |
| [SetHidePivotFieldList](./sethidepivotfieldlist/) | 获取和设置是否隐藏透视表的字段列表。 |
| [GetMaxUniqueItemsPerField](./getmaxuniqueitemsperfield/) | 获取和设置每个字段的唯一项限制 |
| [SetMaxUniqueItemsPerField](./setmaxuniqueitemsperfield/) | 获取和设置每个字段的唯一项限制 |
| [GetUpdateLinksType](./getupdatelinkstype/) | 获取和设置工作簿打开时如何更新外部链接。 |
| [SetUpdateLinksType](./setupdatelinkstype/) | 获取和设置工作簿打开时如何更新外部链接。 |
| [SetPageOrientationType](./setpageorientationtype/) | 设置整个工作簿的打印方向类型。 |
| [GetMaxRow](./getmaxrow/) | 获取最大行索引，基于零。 |
| [GetMaxColumn](./getmaxcolumn/) | 获取最大列索引，基于零。 |
| [GetSmartTagOptions](./getsmarttagoptions/) | 获取智能标签的选项。 |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | 获取此工作簿样式相关属性默认值的设置。 |
| [GetWindowLeft](./getwindowleft/) | 客户端区域左边缘到窗口左边缘的距离，单位为点。 |
| [SetWindowLeft](./setwindowleft/) | 客户端区域左边缘到窗口左边缘的距离，单位为点。 |
| [GetWindowLeftInch](./getwindowleftinch/) | 客户端区域左边缘到窗口左边缘的距离，单位为英寸。 |
| [SetWindowLeftInch](./setwindowleftinch/) | 客户端区域左边缘到窗口左边缘的距离，单位为英寸。 |
| [GetWindowLeftCM](./getwindowleftcm/) | 客户端区域左边缘到窗口左边缘的距离，单位为厘米。 |
| [SetWindowLeftCM](./setwindowleftcm/) | 客户端区域左边缘到窗口左边缘的距离，单位为厘米。 |
| [GetWindowTop](./getwindowtop/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为点。 |
| [SetWindowTop](./setwindowtop/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为点。 |
| [GetWindowTopInch](./getwindowtopinch/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为英寸。 |
| [SetWindowTopInch](./setwindowtopinch/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为英寸。 |
| [GetWindowTopCM](./getwindowtopcm/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为厘米。 |
| [SetWindowTopCM](./setwindowtopcm/) | 客户端区域顶边缘到窗口顶边缘的距离，单位为厘米。 |
| [GetWindowWidth](./getwindowwidth/) | 窗口的宽度，单位为点。 |
| [SetWindowWidth](./setwindowwidth/) | 窗口的宽度，单位为点。 |
| [GetWindowWidthInch](./getwindowwidthinch/) | 窗口的宽度，单位为英寸。 |
| [SetWindowWidthInch](./setwindowwidthinch/) | 窗口的宽度，单位为英寸。 |
| [GetWindowWidthCM](./getwindowwidthcm/) | 窗口的宽度，单位为厘米。 |
| [SetWindowWidthCM](./setwindowwidthcm/) | 窗口的宽度，单位为厘米。 |
| [GetWindowHeight](./getwindowheight/) | 窗口的高度，单位为点。 |
| [SetWindowHeight](./setwindowheight/) | 窗口的高度，单位为点。 |
| [GetWindowHeightInch](./getwindowheightinch/) | 窗口的高度，单位为英寸。 |
| [SetWindowHeightInch](./setwindowheightinch/) | 窗口的高度，单位为英寸。 |
| [GetWindowHeightCM](./getwindowheightcm/) | 窗口的高度，单位为厘米。 |
| [SetWindowHeightCM](./setwindowheightcm/) | 窗口的高度，单位为厘米。 |
| [GetUpdateAdjacentCellsBorder](./getupdateadjacentcellsborder/) | 指示是否更新相邻单元格的边框。 |
| [SetUpdateAdjacentCellsBorder](./setupdateadjacentcellsborder/) | 指示是否更新相邻单元格的边框。 |
| [GetSignificantDigitsType](./getsignificantdigitstype/) | 获取和设置此工作簿中输出数值的有效数字类型。默认值为 CellsHelper.SignificantDigitsType。 |
| [SetSignificantDigitsType](./setsignificantdigitstype/) | 获取和设置此工作簿中输出数值的有效数字类型。默认值为 CellsHelper.SignificantDigitsType。 |
| [GetCheckCompatibility](./getcheckcompatibility/) | 指示在保存工作簿时是否检查与早期版本的兼容性。 |
| [SetCheckCompatibility](./setcheckcompatibility/) | 指示在保存工作簿时是否检查与早期版本的兼容性。 |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。 |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。 |
| [GetAutoRecover](./getautorecover/) | 指示文件是否标记为自动恢复。 |
| [SetAutoRecover](./setautorecover/) | 指示文件是否标记为自动恢复。 |
| [GetCrashSave](./getcrashsave/) | 指示应用程序在崩溃后是否最后保存了工作簿文件。 |
| [SetCrashSave](./setcrashsave/) | 指示应用程序在崩溃后是否最后保存了工作簿文件。 |
| [GetDataExtractLoad](./getdataextractload/) | 指示应用程序上次是否为数据恢复打开了工作簿。 |
| [SetDataExtractLoad](./setdataextractload/) | 指示应用程序上次是否为数据恢复打开了工作簿。 |
| [GetRepairLoad](./getrepairload/) | 指示应用程序上次是否以安全模式或修复模式打开了工作簿。 |
| [SetRepairLoad](./setrepairload/) | 指示应用程序上次是否以安全模式或修复模式打开了工作簿。 |
| [GetBuildVersion](./getbuildversion/) | 指定应用程序的增量公开发布版本。 |
| [SetBuildVersion](./setbuildversion/) | 指定应用程序的增量公开发布版本。 |
| [GetMemorySetting](./getmemorysetting/) | 获取或设置内存使用选项。新选项将作为新建工作表的默认选项，但对已有工作表不生效。 |
| [SetMemorySetting](./setmemorysetting/) | 获取或设置内存使用选项。新选项将作为新建工作表的默认选项，但对已有工作表不生效。 |
| [GetPaperSize](./getpapersize/) | 获取和设置默认打印纸张尺寸。 |
| [SetPaperSize](./setpapersize/) | 获取和设置默认打印纸张尺寸。 |
| [GetMaxRowsOfSharedFormula](./getmaxrowsofsharedformula/) | 获取和设置共享公式的最大行号。 |
| [SetMaxRowsOfSharedFormula](./setmaxrowsofsharedformula/) | 获取和设置共享公式的最大行号。 |
| [GetCompliance](./getcompliance/) | 指定输出文档的 OOXML 版本。默认值为 Ecma376_2006。 |
| [SetCompliance](./setcompliance/) | 指定输出文档的 OOXML 版本。默认值为 Ecma376_2006。 |
| [GetQuotePrefixToStyle](./getquoteprefixtostyle/) | 指示在将以单引号开头的字符串值输入到单元格时是否设置 Style.QuotePrefix 属性。 |
| [SetQuotePrefixToStyle](./setquoteprefixtostyle/) | 指示在将以单引号开头的字符串值输入到单元格时是否设置 Style.QuotePrefix 属性。 |
| [GetFormulaSettings](./getformulasettings/) | 获取公式相关功能的设置。 |
| [GetPropertiesFollowChartPoint](./getpropertiesfollowchartpoint/) | 指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。 |
| [SetPropertiesFollowChartPoint](./setpropertiesfollowchartpoint/) | 指示此工作簿中所有图表的数据点属性和数据标签是否遵循其引用。 |
| [GetDiscardImageEditData](./getdiscardimageeditdata/) | 指示是否丢弃编辑的图像数据。 |
| [SetDiscardImageEditData](./setdiscardimageeditdata/) | 指示是否丢弃编辑的图像数据。 |
| [GetDefaultImageResolution](./getdefaultimageresolution/) | 获取和设置图像的默认分辨率。 |
| [SetDefaultImageResolution](./setdefaultimageresolution/) | 获取和设置图像的默认分辨率。 |
| [GetWpsCompatibility](./getwpscompatibility/) | 指示是否兼容 WPS。 |
| [SetWpsCompatibility](./setwpscompatibility/) | 指示是否兼容 WPS。 |
