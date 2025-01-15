---
title: GetStringValue Method 
linktitle: GetStringValue
second_title: Aspose.Cells for Go via C++ API Reference
description: 'GetStringValue method. Encapsulates the function that represents getstringvalue in Go.'
type: docs
weight: 200
url: /go-cpp/cell/getstringvalue/
---

## GetStringValue function

Gets the string value contained in the cell. If the type of this cell is string, then return the string value itself.For other cell types, the formatted string value (formatted with the specified style of this cell) will be returned.The formatted cell value is same with what you can get from excel when copying a cell as text(such ascopying cell to text editor or exporting to csv).

```go

func (instance *Cell) GetStringValue()  (string,  error) 

```

## Remarks


## See Also

* Class [Cell](../)
* Library [Aspose.Cells for Go](../../)
