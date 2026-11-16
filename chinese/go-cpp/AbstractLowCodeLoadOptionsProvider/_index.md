---
title: "AbstractLowCodeLoadOptionsProvider 类"
linktitle: "AbstractLowCodeLoadOptionsProvider"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "AbstractLowCodeLoadOptionsProvider 类。封装表示 Go 中 abstractlowcodeloadoptionsprovider 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/abstractlowcodeloadoptionsprovider/
---

## AbstractLowCodeLoadOptionsProvider class

实现为使用多个输入（如模板文件）的进程提供多种加载选项。

```go

type AbstractLowCodeLoadOptionsProvider struct  {
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
| [MoveNext](./movenext/) | 检查是否还有更多输入。 |
| [GetCurrent](./getcurrent/) | 获取用于加载当前处理部分数据的加载选项。 |
| [Finish](./finish/) | 在处理当前输入部分后释放资源。 |
