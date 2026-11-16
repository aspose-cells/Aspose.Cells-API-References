---
title: "VbaProjectReferenceCollection 类"
linktitle: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "VbaProjectReferenceCollection 类。封装在 Go 中表示 vbaprojectreferencecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/vbaprojectreferencecollection/
---

## VbaProjectReferenceCollection class

表示 VBA 项目的所有引用。

```go

type VbaProjectReferenceCollection struct  {
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
| [Get](./get/) | 通过索引获取列表中的引用。 |
| [AddRegisteredReference](./addregisteredreference/) | 添加对 Automation 类型库的引用。 |
| [AddControlReferernce](./addcontrolreferernce/) | 添加对 twiddled 类型库及其扩展类型库的引用。 |
| [AddProjectReferernce](./addprojectreferernce/) | 添加对外部 VBA 项目的引用。 |
| [Copy](./copy/) | 从其他 VBA 项目复制引用。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
