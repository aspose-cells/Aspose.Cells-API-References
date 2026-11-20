---
title: CellsAI.AskAsync
second_title: Aspose.Cells for .NET API Reference
description: "CellsAI method. Answers a question about a workbook, with supporting citations."
type: docs
url: /net/aspose.cells.ai/cellsai/askasync/
---
## CellsAI.AskAsync method

Answers a question about a workbook, with supporting citations.

```csharp
public Task<WorkbookAnswerResult> AskAsync(Workbook workbook, string question, WorkbookContentOptions? options = null, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook to process. |
| question | String | The question to answer. |
| options | WorkbookContentOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a WorkbookAnswerResult.

### See Also

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
