---
title: Class WorkbookAnswerResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookAnswerResult class. The result of AskAsync."
type: docs
url: /net/aspose.cells.ai/workbookanswerresult/
---
## WorkbookAnswerResult class

The result of AskAsync.

```csharp
public sealed class WorkbookAnswerResult : CellsAIResult
```

## Properties

| Name | Description |
| --- | --- |
| [Answer](answer/) { get; } | The answer generated from the workbook content. |
| [Citations](citations/) { get; } | The citations supporting the answer. Never null. |
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
