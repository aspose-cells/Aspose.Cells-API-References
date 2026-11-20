---
title: CellsAI.EditAsync
second_title: Aspose.Cells for .NET API Reference
description: "CellsAI method. Edits a copy of the workbook according to instructions and returns the new workbook. The input workbook is never modified."
type: docs
url: /net/aspose.cells.ai/cellsai/editasync/
---
## CellsAI.EditAsync method

Edits a copy of the workbook according to instructions and returns the new workbook. The input workbook is never modified.

```csharp
public Task<WorkbookEditResult> EditAsync(Workbook workbook, string instructions, WorkbookEditOptions options, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook to process. |
| instructions | String | The natural-language instructions that describe the requested change. |
| options | WorkbookEditOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a WorkbookEditResult.

### See Also

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
