---
title: "VbaModuleCollection 类"
linktitle: "VbaModuleCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "VbaModuleCollection 类。封装在 Go 中表示 vbamodulecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/vbamodulecollection/
---

## VbaModuleCollection class

表示 <see cref="VbaModule"/> 的列表

```go

type VbaModuleCollection struct  {
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
|[AddDesignerStorage](./adddesignerstorage/) |  | 
| [GetDesignerStorage](./getdesignerstorage/) | 表示 Designer 的数据。 |
| [Add_Worksheet](./add_worksheet/) | 为工作表添加模块。 |
| [Add_VbaModuleType_String](./add_vbamoduletype_string/) | 添加模块。 |
| [AddUserForm](./adduserform/) | 将用户表单插入到 VBA 项目中。 |
| [Get_Int](./get_int/) | 通过索引获取列表中的 VbaModule。 |
| [Remove_Worksheet](./remove_worksheet/) | 移除工作表的模块。 |
| [Remove_String](./remove_string/) | 按名称移除模块 |
| [Get_String](./get_string/) | 通过名称获取列表中的 VbaModule。 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
