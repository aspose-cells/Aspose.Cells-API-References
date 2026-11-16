---
title: "SqlScriptSaveOptions 类"
linktitle: "SqlScriptSaveOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SqlScriptSaveOptions 类。封装表示 Go 中 sqlscriptsaveoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

表示保存 SQL 的选项。

```go

type SqlScriptSaveOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | 创建用于保存 SQL 文件的选项。 |
| [NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetCheckIfTableExists](./getcheckiftableexists/) | 在创建之前检查表名是否已存在 |
| [SetCheckIfTableExists](./setcheckiftableexists/) | 在创建之前检查表名是否已存在 |
| [GetColumnTypeMap](./getcolumntypemap/) | 获取并设置不同数据库的列类型映射。 |
| [SetColumnTypeMap](./setcolumntypemap/) | 获取并设置不同数据库的列类型映射。 |
| [GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | 检查所有数据以查找列的数据类型。 |
| [SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | 检查所有数据以查找列的数据类型。 |
| [GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | 在每条数据之间插入空行。 |
| [SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | 在每条数据之间插入空行。 |
| [GetSeparator](./getseparator/) | 获取并设置 SQL 脚本的字符分隔符。 |
| [SetSeparator](./setseparator/) | 获取并设置 SQL 脚本的字符分隔符。 |
| [GetOperatorType](./getoperatortype/) | 获取并设置 SQL 的运算符类型。 |
| [SetOperatorType](./setoperatortype/) | 获取并设置 SQL 的运算符类型。 |
| [GetPrimaryKey](./getprimarykey/) | 表示数据表中哪一列是主键。 |
| [SetPrimaryKey](./setprimarykey/) | 表示数据表中哪一列是主键。 |
| [GetCreateTable](./getcreatetable/) | 指示是否导出创建表的 SQL。 |
| [SetCreateTable](./setcreatetable/) | 指示是否导出创建表的 SQL。 |
| [GetIdName](./getidname/) | 获取并设置 ID 列的名称。 |
| [SetIdName](./setidname/) | 获取并设置 ID 列的名称。 |
| [GetStartId](./getstartid/) | 获取并设置起始 ID。 |
| [SetStartId](./setstartid/) | 获取并设置起始 ID。 |
| [GetTableName](./gettablename/) | 获取并设置表名。 |
| [SetTableName](./settablename/) | 获取并设置表名。 |
| [GetExportAsString](./getexportasstring/) | 指示是否将所有数据导出为字符串值。 |
| [SetExportAsString](./setexportasstring/) | 指示是否将所有数据导出为字符串值。 |
| [GetSheetIndexes](./getsheetindexes/) | 表示导出工作表的索引。 |
| [SetSheetIndexes](./setsheetindexes/) | 表示导出工作表的索引。 |
| [GetExportArea](./getexportarea/) | 获取或设置导出范围。 |
| [SetExportArea](./setexportarea/) | 获取或设置导出范围。 |
| [GetHasHeaderRow](./gethasheaderrow/) | 指示范围是否包含标题行。 |
| [SetHasHeaderRow](./sethasheaderrow/) | 指示范围是否包含标题行。 |
| [GetSaveFormat](./getsaveformat/) | 获取保存文件的格式。 |
| [GetClearData](./getcleardata/) | 在保存文件后使工作簿为空。 |
| [SetClearData](./setcleardata/) | 在保存文件后使工作簿为空。 |
| [GetCachedFileFolder](./getcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [SetCachedFileFolder](./setcachedfilefolder/) | 用于临时文件的文件夹，可用作数据缓存。 |
| [GetValidateMergedAreas](./getvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [SetValidateMergedAreas](./setvalidatemergedareas/) | 指示是否在保存文件前验证合并单元格。 |
| [GetMergeAreas](./getmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [SetMergeAreas](./setmergeareas/) | 指示是否在保存文件前合并条件格式和验证的区域。 |
| [GetCreateDirectory](./getcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [SetCreateDirectory](./setcreatedirectory/) | 如果为 true 且目录不存在，目录将在保存文件前自动创建。 |
| [GetSortNames](./getsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [SetSortNames](./setsortnames/) | 指示是否在保存文件前对已定义名称进行排序。 |
| [GetSortExternalNames](./getsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [SetSortExternalNames](./setsortexternalnames/) | 指示是否在保存文件前对外部已定义名称进行排序。 |
| [GetRefreshChartCache](./getrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [SetRefreshChartCache](./setrefreshchartcache/) | 指示是否缓存图表的最新数据。 |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当输入的值超过 32K 时，将被截断。 |
| [GetUpdateSmartArt](./getupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [SetUpdateSmartArt](./setupdatesmartart/) | 指示是否更新 Smart Art 设置。默认值为 false。 |
| [GetEncryptDocumentProperties](./getencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
| [SetEncryptDocumentProperties](./setencryptdocumentproperties/) | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。 |
