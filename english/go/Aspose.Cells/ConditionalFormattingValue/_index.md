---
title: ConditionalFormattingValue Class 
linktitle: ConditionalFormattingValue
second_title: Aspose.Cells for Go API Reference
description: 'ConditionalFormattingValue class. Encapsulates the object that represents conditionalformattingvalue in Go.'
type: docs
weight: 200
url: /go/aspose.cells/conditionalformattingvalue/
---

## ConditionalFormattingValue class

Describes the values of the interpolation points in a gradient scale, dataBar or iconSet.

```go

type ConditionalFormattingValue struct 

conditionalformattingvalue, _ := asposecells.NewConditionalFormattingValue()

```

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetType](./gettype/) | Get or set the type of this conditional formatting value object.Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Maxwill auto set "Value" to null. | 
|[SetType](./settype/) | Get or set the type of this conditional formatting value object.Setting the type to FormatConditionValueType.Min or FormatConditionValueType.Maxwill auto set "Value" to null. | 
|[IsGTE](./isgte/) | Get or set the Greater Than Or Equal flag.Use only for icon sets, determines whether this threshold value usesthe greater than or equal to operator.'false' indicates 'greater than' is used instead of 'greater than or equal to'.Default value is true. | 
|[SetIsGTE](./setisgte/) | Get or set the Greater Than Or Equal flag.Use only for icon sets, determines whether this threshold value usesthe greater than or equal to operator.'false' indicates 'greater than' is used instead of 'greater than or equal to'.Default value is true. | 
