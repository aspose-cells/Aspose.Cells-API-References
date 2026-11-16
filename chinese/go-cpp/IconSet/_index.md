---
title: "IconSet 类"
linktitle: "IconSet"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "IconSet 类。封装在 Go 中表示 iconset 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/iconset/
---

## IconSet class

描述 IconSet 条件格式化规则。此条件格式化规则根据单元格的值为其应用图标。

```go

type IconSet struct  {
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
| [GetCfIcons](./getcficons/) | 从集合中获取 theConditionalFormattingIcon |
| [GetCfvos](./getcfvos/) | 获取 CFValueObjects 实例。 |
| [GetType](./gettype/) | 获取或设置要显示的图标集类型。设置类型时将自动检查当前 Cfvos 的计数是否与新类型一致。如果不一致，旧的 Cfvos 将被清除，并添加默认 Cfvos。 |
| [SetType](./settype/) | 获取或设置要显示的图标集类型。设置类型时将自动检查当前 Cfvos 的计数是否与新类型一致。如果不一致，旧的 Cfvos 将被清除，并添加默认 Cfvos。 |
| [IsCustom](./iscustom/) | 指示图标集是否为自定义。默认值为 false。 |
| [GetShowValue](./getshowvalue/) | 获取或设置标志，指示是否显示此图标集所应用单元格的值。默认值为 true。 |
| [SetShowValue](./setshowvalue/) | 获取或设置标志，指示是否显示此图标集所应用单元格的值。默认值为 true。 |
| [GetReverse](./getreverse/) | 获取或设置标志，指示是否反转此图标集中的图标默认顺序。默认值为 false。 |
| [SetReverse](./setreverse/) | 获取或设置标志，指示是否反转此图标集中的图标默认顺序。默认值为 false。 |
