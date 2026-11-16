---
title: "ReferredArea 类"
linktitle: "ReferredArea"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ReferredArea 类。封装在 Go 中表示 referredarea 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/referredarea/
---

## ReferredArea class

表示公式引用的区域。

```go

type ReferredArea struct  {
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
| [IsExternalLink](./isexternallink/) | 指示此是否为外部链接。 |
| [GetExternalFileName](./getexternalfilename/) | 如果这是外部引用，则获取外部文件名。 |
| [GetSheetName](./getsheetname/) | 指示此引用所在的工作表。 |
| [GetSheetNames](./getsheetnames/) | 此实例引用的所有工作表的名称。 |
| [IsEntireRow](./isentirerow/) | 指示此区域是否包含所有列（整行）。 |
| [IsEntireColumn](./isentirecolumn/) | 指示此区域是否包含所有行（整列）。 |
| [IsArea](./isarea/) | 指示此是否为区域。 |
| [GetEndColumn](./getendcolumn/) | 该区域的结束列。 |
| [GetStartColumn](./getstartcolumn/) | 区域的起始列。 |
| [GetEndRow](./getendrow/) | 区域的结束行。 |
| [GetStartRow](./getstartrow/) | 区域的起始行。 |
| [GetValues](./getvalues/) | 获取此区域中的单元格值。 |
| [GetValues_Bool](./getvalues_bool/) | 获取此区域中的单元格值。 |
| [GetValue_Int_Int](./getvalue_int_int/) | 获取相对于此区域左上角给定偏移量的单元格值。 |
| [GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | 获取相对于此区域左上角给定偏移量的单元格值。 |
| [ToString](./tostring/) | 返回此区域的引用地址。通常它是可在公式中使用的引用地址，例如 "Sheet1!A1:C3"。 |
