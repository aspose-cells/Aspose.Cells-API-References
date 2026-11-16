---
title: "GetSheetsInLoadingOrder 方法"
linktitle: "GetSheetsInLoadingOrder"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "GetSheetsInLoadingOrder 方法。封装了在 Go 中表示 getsheetsinloadingorder 的函数。"
type: docs
weight: 200
url: /zh/go-cpp/loadfilter/getsheetsinloadingorder/
---

## GetSheetsInLoadingOrder function

指定要加载的工作表（索引）及其顺序。默认值为 null，表示加载模板文件中按默认顺序的所有工作表。如果不为 null 且某些工作表的索引不在返回的数组中，则该工作表将不会被加载。

```go

func (instance *LoadFilter) GetSheetsInLoadingOrder()  ([]int32,  error) 

```

## 备注


## 另请参阅

* Class [LoadFilter](../)
* Library [Aspose.Cells for Go](../../)
