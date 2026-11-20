---
title: CellsAI.GenerateFormulaAsync
second_title: Aspose.Cells for .NET API Reference
description: "CellsAI method. Generates a formula for a target cell that passes the Aspose.Cells parser and calculation engine validation. The input workbook is not modified."
type: docs
url: /net/aspose.cells.ai/cellsai/generateformulaasync/
---
## CellsAI.GenerateFormulaAsync method

Generates a formula for a target cell that passes the Aspose.Cells parser and calculation engine validation. The input workbook is not modified.

```csharp
public Task<FormulaGenerationResult> GenerateFormulaAsync(Cell targetCell, string instructions, WorkbookContentOptions? options = null, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| targetCell | Cell | The cell for which a formula is generated. |
| instructions | String | The natural-language instructions that describe the requested change. |
| options | WorkbookContentOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a FormulaGenerationResult.

### See Also

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
