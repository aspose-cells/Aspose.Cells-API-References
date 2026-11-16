---
title: "GetValuesField 方法"
linktitle: "GetValuesField"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetValuesField 方法。封装了在 Go 中表示 getvaluesfield 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/pivottable/getvaluesfield/
---

## GetValuesField function

获取一个表示 PivotTable 中所有数据字段的 PivotField 对象。只读。当 Data 区域中有两个或以上数据字段时才会创建。默认位于行区域。您可以使用 PivotTable.AddFieldToArea() 方法将其拖动到行/列区域。

```go

func (instance *PivotTable) GetValuesField()  (*PivotField,  error) 

```

## 备注


## 另请参阅

* Class [PivotTable](../)
* Library [Aspose.Cells for Go](../../)
