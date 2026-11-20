---
title: Class WorkbookInspectionResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookInspectionResult class. The result of InspectAsync."
type: docs
url: /net/aspose.cells.ai/workbookinspectionresult/
---
## WorkbookInspectionResult class

The result of InspectAsync.

```csharp
public sealed class WorkbookInspectionResult : CellsAIResult
```

## Properties

| Name | Description |
| --- | --- |
| [Findings](findings/) { get; } | The findings of the inspection. Never null. |
| [Operation](operation/) { get; } | Gets the operation that produced this result. |
| [Text](text/) { get; } | Gets the human-readable representation of the result. |

## Inherited Members

### Inherited Properties

| Name | Description |
| --- | --- |
| [Usage](../cellsairesult/usage/) { get; } | Usage information for the operation. |
| [Warnings](../cellsairesult/warnings/) { get; } | Non-fatal warnings. Never null; empty when there are none. |

### Inherited Methods

| Name | Description |
| --- | --- |
| [ToString](../cellsairesult/tostring/)() | Returns the human-readable representation of the result. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
