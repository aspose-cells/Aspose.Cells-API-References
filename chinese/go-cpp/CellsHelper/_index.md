---
title: "CellsHelper 类"
linktitle: "CellsHelper"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "CellsHelper 类。封装在 Go 中表示 cellshelper 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cellshelper/
---

## CellsHelper class

提供辅助函数。

```go

type CellsHelper struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [CellsHelper_GetSignificantDigitsType](./cellshelper_getsignificantdigitstype/) | 获取和设置用于输出数值的默认有效数字类型。默认值为 SignificantDigitsType.G17。 |
| [CellsHelper_SetSignificantDigitsType](./cellshelper_setsignificantdigitstype/) | 获取和设置用于输出数值的默认有效数字类型。默认值为 SignificantDigitsType.G17。 |
| [CellsHelper_GetDPI](./cellshelper_getdpi/) | 获取机器的 DPI。 |
| [CellsHelper_SetDPI](./cellshelper_setdpi/) | 获取机器的 DPI。 |
| [CellsHelper_GetTextWidth](./cellshelper_gettextwidth/) | 获取文本的宽度（单位为点）。 |
| [CellsHelper_GetVersion](./cellshelper_getversion/) | 获取发行版本。 |
| [CellsHelper_CellNameToIndex](./cellshelper_cellnametoindex/) | 根据单元格名称获取其行和列索引。 |
| [CellsHelper_CellIndexToName](./cellshelper_cellindextoname/) | 根据行列索引获取单元格名称。 |
| [CellsHelper_ColumnIndexToName](./cellshelper_columnindextoname/) | 根据列索引获取列名称。 |
| [CellsHelper_ColumnNameToIndex](./cellshelper_columnnametoindex/) | 根据列名称获取列索引。 |
| [CellsHelper_RowIndexToName](./cellshelper_rowindextoname/) | 根据行索引获取行名称。 |
| [CellsHelper_RowNameToIndex](./cellshelper_rownametoindex/) | 根据行名称获取行索引。 |
| [CellsHelper_GetDateTimeFromDouble](./cellshelper_getdatetimefromdouble/) | 将 double 值转换为日期时间值。 |
| [CellsHelper_GetDoubleFromDateTime](./cellshelper_getdoublefromdatetime/) | 将日期时间转换为 double 值。 |
| [CellsHelper_GetStartupPath](./cellshelper_getstartuppath/) | 获取或设置启动路径，该路径会被某些外部公式引用。 |
| [CellsHelper_SetStartupPath](./cellshelper_setstartuppath/) | 获取或设置启动路径，该路径会被某些外部公式引用。 |
| [CellsHelper_GetAltStartPath](./cellshelper_getaltstartpath/) | 获取或设置备用启动路径，该路径会被某些外部公式引用。 |
| [CellsHelper_SetAltStartPath](./cellshelper_setaltstartpath/) | 获取或设置备用启动路径，该路径会被某些外部公式引用。 |
| [CellsHelper_GetLibraryPath](./cellshelper_getlibrarypath/) | 获取或设置库路径，该路径会被某些外部公式引用。 |
| [CellsHelper_SetLibraryPath](./cellshelper_setlibrarypath/) | 获取或设置库路径，该路径会被某些外部公式引用。 |
| [CellsHelper_GetUsedColors](./cellshelper_getusedcolors/) | 获取工作簿中使用的所有颜色。 |
| [CellsHelper_MergeFiles](./cellshelper_mergefiles/) | 将多个大型 xls 文件合并为一个 xls 文件。 |
| [CellsHelper_GetCacheFolder](./cellshelper_getcachefolder/) | 获取可能用作数据缓存的临时文件夹。 |
| [CellsHelper_SetCacheFolder](./cellshelper_setcachefolder/) | 设置可能用作数据缓存的临时文件夹。 |
| [CellsHelper_CreateSafeSheetName_String](./cellshelper_createsafesheetname_string/) | 检查给定的工作表名称，并在需要时创建有效名称。如果给定的工作表名称符合 Excel 工作表名称规则，则返回该名称。否则，如果长度超过限制，则会截断字符串，并将无效字符替换为 ' '，然后返回重建后的字符串值。 |
| [CellsHelper_CreateSafeSheetName_String_Char](./cellshelper_createsafesheetname_string_char/) | 检查给定的工作表名称，并在需要时创建有效名称。如果给定的工作表名称符合 Excel 工作表名称规则，则返回该名称。否则，如果长度超过限制，则会截断字符串，并将无效字符替换为给定的字符，然后返回重建后的字符串值。 |
| [CellsHelper_NeedQuoteInFormula](./cellshelper_needquoteinformula/) | 指示工作表名称是否应使用单引号括起来 |
| [CellsHelper_IsCloudPlatform](./cellshelper_iscloudplatform/) | 在云平台（如 Azure、AWSLambda 等）上运行时，请将此属性设为 True， |
| [CellsHelper_SetIsCloudPlatform](./cellshelper_setiscloudplatform/) | 在云平台（如 Azure、AWSLambda 等）上运行时，请将此属性设为 True， |
