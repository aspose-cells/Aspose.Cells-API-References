---
title: "ErrorCheckOption 类"
linktitle: "ErrorCheckOption"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ErrorCheckOption 类。封装在 Go 中表示 errorcheckoption 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/errorcheckoption/
---

## ErrorCheckOption class

对特定范围应用的错误检查设置。

```go

type ErrorCheckOption struct  {
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
| [IsErrorCheck](./iserrorcheck/) | 检查给定的错误类型是否将被检查。 |
| [SetErrorCheck](./seterrorcheck/) | 设置是否检查给定的错误类型。 |
| [GetCountOfRange](./getcountofrange/) | 获取受此设置影响的范围数量。 |
| [AddRange](./addrange/) | 通过此设置添加一个受影响的范围。 |
| [GetRange](./getrange/) | 获取此设置在给定索引处的受影响范围。 |
| [RemoveRange](./removerange/) | 通过给定索引删除一个范围。 |
