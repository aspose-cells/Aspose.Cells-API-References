---
title: Class CellsAIResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAIResult class. The base class of all Cells AI operation results. Instances are immutable objects with no public constructors."
type: docs
url: /net/aspose.cells.ai/cellsairesult/
---
## CellsAIResult class

The base class of all Cells AI operation results. Instances are immutable objects with no public constructors.

```csharp
public abstract class CellsAIResult
```

## Properties

| Name | Description |
| --- | --- |
| [Operation](operation/) { get; } | The operation that produced this result. Useful for logging and for deciding how to present a result without pattern matching on its concrete type. |
| [Text](text/) { get; } | A human-readable representation of the result, suitable for direct display. Never null; empty when the operation produced no displayable content. Structured data remains available on the concrete result type. |
| [Usage](usage/) { get; } | Usage information for the operation. |
| [Warnings](warnings/) { get; } | Non-fatal warnings. Never null; empty when there are none. |

## Methods

| Name | Description |
| --- | --- |
| [ToString](tostring/)() | Returns the human-readable representation of the result. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
