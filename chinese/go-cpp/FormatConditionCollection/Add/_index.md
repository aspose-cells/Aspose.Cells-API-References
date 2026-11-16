---
title: "Add 方法"
linktitle: "添加"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Add 方法。封装了在 Go 中表示 add 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/formatconditioncollection/add/
---

## Add function

向 FormatConditions 添加一个格式条件和受影响的单元格范围。FormatConditions 最多可以包含三个条件格式。条件格式的公式中不允许引用其他工作表。

```go

func (instance *FormatConditionCollection) Add(cellarea *CellArea, type_ FormatConditionType, operatortype OperatorType, formula1 string, formula2 string)  ([]int32,  error) 

```

## 备注


## 另请参阅

* Class [FormatConditionCollection](../)
* Library [Aspose.Cells for Go](../../)
