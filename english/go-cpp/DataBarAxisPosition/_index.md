---
title: DataBarAxisPosition Enum 
linktitle: DataBarAxisPosition
second_title: Aspose.Cells for Go via C++ API Reference
description: 'DataBarAxisPosition enum. Encapsulates the object that represents databaraxisposition in Go.'
type: docs
weight: 200
url: /go-cpp/databaraxisposition/
---

## DataBarAxisPosition Enum

Specifies the axis position for a range of cells with conditional formatting as data bars.

```go

type DataBarAxisPosition int32


```

## Fields

| Field | Description |
| --- | --- |
|[Automatic](./automatic/) | Display the axis at a variable position based on the ratio of the minimum negative value to the maximum positive value in the range.Positive values are displayed in a left-to-right direction.Negative values are displayed in a right-to-left direction.When all values are positive or all values are negative, no axis is displayed. | 
|[Midpoint](./midpoint/) | Display the axis at the midpoint of the cell regardless of the set of values in the range.Positive values are displayed in a left-to-right direction.Negative values are displayed in a right-to-left direction. | 
|[None](./none/) | No axis is displayed, and both positive and negative values are displayed in the left-to-right direction. | 
