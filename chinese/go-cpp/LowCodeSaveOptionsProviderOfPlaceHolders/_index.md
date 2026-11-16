---
title: "LowCodeSaveOptionsProviderOfPlaceHolders 类"
linktitle: "LowCodeSaveOptionsProviderOfPlaceHolders"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "LowCodeSaveOptionsProviderOfPlaceHolders 类。封装表示 Go 中 lowcodesaveoptionsproviderofplaceholders 对象。"
type: docs
weight: 200
url: /zh/go-cpp/lowcodesaveoptionsproviderofplaceholders/
---

## LowCodeSaveOptionsProviderOfPlaceHolders class

实现提供保存选项，将拆分部分保存到文件，并且生成文件的路径使用占位符定义。

```go

type LowCodeSaveOptionsProviderOfPlaceHolders struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_String](./newlowcodesaveoptionsproviderofplaceholders_string/) | 实例化一个实例，以根据指定的模板提供保存选项。 |
| [NewLowCodeSaveOptionsProviderOfPlaceHolders_AbstractLowCodeSaveOptionsProvider](./newlowcodesaveoptionsproviderofplaceholders_abstractlowcodesaveoptionsprovider/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSheetIndexOffset](./getsheetindexoffset/) | 文件路径中使用的工作表索引与其实际值（SplitPartInfo.SheetIndex）之间的偏移量。 |
| [SetSheetIndexOffset](./setsheetindexoffset/) | 文件路径中使用的工作表索引与其实际值（SplitPartInfo.SheetIndex）之间的偏移量。 |
| [GetSplitPartIndexOffset](./getsplitpartindexoffset/) | 文件路径中使用的拆分部分索引与其实际值（SplitPartInfo.PartIndex）之间的偏移量。 |
| [SetSplitPartIndexOffset](./setsplitpartindexoffset/) | 文件路径中使用的拆分部分索引与其实际值（SplitPartInfo.PartIndex）之间的偏移量。 |
| [GetBuildPathWithSheetAlways](./getbuildpathwithsheetalways/) | 是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引和名称以及相应前缀（SheetNamePrefix）将不会添加到文件路径中。 |
| [SetBuildPathWithSheetAlways](./setbuildpathwithsheetalways/) | 是否始终将工作表索引或名称添加到文件路径。默认值为 false，即当只有一个工作表时，工作表索引和名称以及相应前缀（SheetNamePrefix）将不会添加到文件路径中。 |
| [GetBuildPathWithSplitPartAlways](./getbuildpathwithsplitpartalways/) | 是否始终将拆分部分索引添加到文件路径。默认值为 false，即当只有一个拆分部分时，拆分部分索引和相应前缀（SplitPartPrefix）将不会添加到文件路径中。 |
| [SetBuildPathWithSplitPartAlways](./setbuildpathwithsplitpartalways/) | 是否始终将拆分部分索引添加到文件路径。默认值为 false，即当只有一个拆分部分时，拆分部分索引和相应前缀（SplitPartPrefix）将不会添加到文件路径中。 |
| [GetSheetNamePrefix](./getsheetnameprefix/) | 工作表索引的前缀。 |
| [SetSheetNamePrefix](./setsheetnameprefix/) | 工作表索引的前缀。 |
| [GetSheetIndexPrefix](./getsheetindexprefix/) | 工作表索引的前缀。 |
| [SetSheetIndexPrefix](./setsheetindexprefix/) | 工作表索引的前缀。 |
| [GetSplitPartPrefix](./getsplitpartprefix/) | 拆分部分索引的前缀。 |
| [SetSplitPartPrefix](./setsplitpartprefix/) | 拆分部分索引的前缀。 |
| [GetSaveOptionsTemplate](./getsaveoptionstemplate/) | 在 GetSaveOptions(SplitPartInfo) 中创建保存选项实例的模板。 |
| [SetSaveOptionsTemplate](./setsaveoptionstemplate/) | 在 GetSaveOptions(SplitPartInfo) 中创建保存选项实例的模板。 |
| [GetSaveOptions](./getsaveoptions/) | 获取用于获取当前拆分部分输出设置的保存选项。 |
| [Finish](./finish/) | 在处理当前拆分部分后释放资源。 |
