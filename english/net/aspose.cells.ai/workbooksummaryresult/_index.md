---
title: Class WorkbookSummaryResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookSummaryResult class. The result of SummarizeAsync."
type: docs
url: /net/aspose.cells.ai/workbooksummaryresult/
---
## WorkbookSummaryResult class

The result of SummarizeAsync.

```csharp
public sealed class WorkbookSummaryResult : CellsAIResult
```

## Properties

| Name | Description |
| --- | --- |
| [Citations](citations/) { get; } | The citations supporting the summary. Never null. |
| [KeyPoints](keypoints/) { get; } | The key points extracted from the workbook. Never null. |
| [Operation](operation/) { get; } | Gets the operation that produced this result. |
| [Summary](summary/) { get; } | The generated summary. |
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
