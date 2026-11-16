---
title: "IndividualFontConfigs 类"
linktitle: "IndividualFontConfigs"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "IndividualFontConfigs 类。封装了在 Go 中表示 individualfontconfigs 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/individualfontconfigs/
---

## IndividualFontConfigs class

每个 <see cref="Workbook"/> 对象的字体配置。

```go

type IndividualFontConfigs struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewIndividualFontConfigs](./newindividualfontconfigs/) | 构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [SetFontSubstitutes](./setfontsubstitutes/) | 为给定的原始字体名称设置字体替代名称。 |
| [GetFontSubstitutes](./getfontsubstitutes/) | 返回一个数组，包含在原始字体不存在时使用的字体替代名称。 |
| [SetFontFolder](./setfontfolder/) | 设置字体文件夹 |
| [SetFontFolders](./setfontfolders/) | 设置字体文件夹集合 |
| [SetFontSources](./setfontsources/) | 设置字体来源。 |
| [GetFontSources](./getfontsources/) | 获取包含来源列表的数组的副本 |
