---
title: "LowCodeSaveOptionsProviderOfAssembling 类"
linktitle: "LowCodeSaveOptionsProviderOfAssembling"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LowCodeSaveOptionsProviderOfAssembling 类。封装了在 Go 中表示 lowcodesaveoptionsproviderofassembling 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/lowcodesaveoptionsproviderofassembling/
---

## LowCodeSaveOptionsProviderOfAssembling class

实现提供保存选项，将拆分部分保存到文件，并且生成文件的路径命名为（可能包含目录）：<see cref=\"PathHeader\"/>+<see cref=\"SheetPrefix\"/>+SheetIndex（或 SheetName）+<see cref=\"SplitPartPrefix\"/>+SplitPartIndex+<see cref=\"PathTail\"/>。

```go

type LowCodeSaveOptionsProviderOfAssembling struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfAssembling](./newlowcodesaveoptionsproviderofassembling/) | 默认构造函数。 |
| [NewLowCodeSaveOptionsProviderOfAssembling_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofassembling_abstractlowcodesaveoptionsprovider/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetPathHeader](./getpathheader/) | 文件路径的头部（在工作表和拆分部分添加内容之前）部分。 |
| [SetPathHeader](./setpathheader/) | 文件路径的头部（在工作表和拆分部分添加内容之前）部分。 |
| [GetPathTail](./getpathtail/) | 文件路径的尾部（在序列号之后）部分。它应包含文件名的扩展名。 |
| [SetPathTail](./setpathtail/) | 文件路径的尾部（在序列号之后）部分。它应包含文件名的扩展名。 |
| [GetUseSheetName](./getusesheetname/) | 是否使用工作表名称而不是工作表索引来构建文件路径。默认值为 false。 |
| [SetUseSheetName](./setusesheetname/) | 是否使用工作表名称而不是工作表索引来构建文件路径。默认值为 false。 |
| [GetSheetPrefix](./getsheetprefix/) | 工作表索引的前缀。 |
| [SetSheetPrefix](./setsheetprefix/) | 工作表索引的前缀。 |
| [GetSplitPartPrefix](./getsplitpartprefix/) | 拆分部分索引的前缀。 |
| [SetSplitPartPrefix](./setsplitpartprefix/) | 拆分部分索引的前缀。 |
| [GetSheetIndexOffset](./getsheetindexoffset/) | 文件路径中使用的工作表索引与其实际值（SplitPartInfo.SheetIndex）之间的偏移量。 |
| [SetSheetIndexOffset](./setsheetindexoffset/) | 文件路径中使用的工作表索引与其实际值（SplitPartInfo.SheetIndex）之间的偏移量。 |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | 文件路径中使用的拆分部分索引与其实际值（SplitPartInfo.PartIndex）之间的偏移量。 |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | 文件路径中使用的拆分部分索引与其实际值（SplitPartInfo.PartIndex）之间的偏移量。 |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | 是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀将不会添加到文件路径中。 |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | 是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引（或名称）及相应前缀将不会添加到文件路径中。 |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | 是否始终将拆分部分索引添加到文件路径。默认值为 false，即当只有一个拆分部分时，拆分部分索引及相应前缀将不会添加到文件路径中。 |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | 是否始终将拆分部分索引添加到文件路径。默认值为 false，即当只有一个拆分部分时，拆分部分索引及相应前缀将不会添加到文件路径中。 |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | 在 GetSaveOptions(SplitPartInfo) 中创建保存选项实例的模板。 |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | 在 GetSaveOptions(SplitPartInfo) 中创建保存选项实例的模板。 |
| [GetSaveOptions](./getsaveoptions/) | 获取用于获取当前拆分部分输出设置的保存选项。 |
| [Finish](./finish/) | 在处理当前拆分部分后释放资源。 |
