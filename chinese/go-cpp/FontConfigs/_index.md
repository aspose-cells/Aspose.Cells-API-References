---
title: "FontConfigs 类"
linktitle: "FontConfigs"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FontConfigs 类。封装了在 Go 中表示 fontconfigs 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/fontconfigs/
---

## FontConfigs class

指定字体设置

```go

type FontConfigs struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewFontConfigs](./newfontconfigs/) | 默认构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [FontConfigs_IsFontAvailable](./fontconfigs_isfontavailable/) | 指示字体是否可用。 |
| [FontConfigs_GetFontFileDataInfo](./fontconfigs_getfontfiledatainfo/) | 获取字体文件数据的信息。 |
| [FontConfigs_GetDefaultFontName](./fontconfigs_getdefaultfontname/) | 获取或设置默认字体名称。 |
| [FontConfigs_SetDefaultFontName](./fontconfigs_setdefaultfontname/) | 获取或设置默认字体名称。 |
| [FontConfigs_GetPreferSystemFontSubstitutes](./fontconfigs_getprefersystemfontsubstitutes/) | 指示在字体不存在且未设置该字体的替代品时，是否优先使用系统字体替代。例如，在 Ubuntu 上，"Arial" 字体通常会被 "Liberation Sans" 替代。默认值为 false。 |
| [FontConfigs_SetPreferSystemFontSubstitutes](./fontconfigs_setprefersystemfontsubstitutes/) | 指示在字体不存在且未设置该字体的替代品时，是否优先使用系统字体替代。例如，在 Ubuntu 上，"Arial" 字体通常会被 "Liberation Sans" 替代。默认值为 false。 |
| [FontConfigs_SetFontSubstitutes](./fontconfigs_setfontsubstitutes/) | 给定原始字体名称的字体替代名称。 |
| [FontConfigs_GetFontSubstitutes](./fontconfigs_getfontsubstitutes/) | 返回一个数组，包含在原始字体不存在时使用的字体替代名称。 |
| [FontConfigs_SetFontFolder](./fontconfigs_setfontfolder/) | 设置字体文件夹 |
| [FontConfigs_SetFontFolders](./fontconfigs_setfontfolders/) | 设置字体文件夹 |
| [FontConfigs_SetFontSources](./fontconfigs_setfontsources/) | 设置字体来源。 |
| [FontConfigs_GetFontSources](./fontconfigs_getfontsources/) | 获取包含来源列表的数组的副本 |
