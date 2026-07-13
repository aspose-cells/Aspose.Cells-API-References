---
title: ChartSplitType Enum 
linktitle: ChartSplitType
second_title: Aspose.Cells for Go via C++ API Reference
description: 'ChartSplitType enum. Encapsulates the object that represents chartsplittype in Go.'
type: docs
weight: 200
url: /go-cpp/chartsplittype/
---

## ChartSplitType Enum

Represents the way the two sections of either a pie of pie chart or a bar of pie chart are split.

```go

type ChartSplitType int32


```

## Fields

| Field | Description |
| --- | --- |
|[Position](./position/) | Represents the data points.The data points shall be split between the pie and the second chart by putting the last split position of the data points in the second chart. | 
|[Value](./value/) | Represents the data points shall be split between the pieand the second chart by putting the data points withvalue less than Split Position in the second chart. | 
|[PercentValue](./percentvalue/) | Represents the data points that shall be split between the pie and the second chart by putting the points with a percentage less than the Split Position percent in the second chart. | 
|[Custom](./custom/) | Represents the data points shall be split between the pieand the second chart according to the Custom Splitvalues. | 
|[Auto](./auto/) | Represents the data points that shall be split using the default mechanism for this chart type. | 
