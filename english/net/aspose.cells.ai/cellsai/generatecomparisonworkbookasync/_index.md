---
title: CellsAI.GenerateComparisonWorkbookAsync
second_title: Aspose.Cells for .NET API Reference
description: "CellsAI method. Compares two workbooks and produces a marked-up workbook that visualizes the differences the way document comparison tools do: inserted content is blue, deleted content is red, and cells whose value is unchanged but whose formatting differs are green. A changed cell shows the new value followed by the old value inside the same cell. The returned workbook can be saved by the caller, e.g. workbook.Save(\"result.xlsx\")."
type: docs
url: /net/aspose.cells.ai/cellsai/generatecomparisonworkbookasync/
---
## CellsAI.GenerateComparisonWorkbookAsync method

Compares two workbooks and produces a marked-up workbook that visualizes the differences the way document comparison tools do: inserted content is blue, deleted content is red, and cells whose value is unchanged but whose formatting differs are green. A changed cell shows the new value followed by the old value inside the same cell. The returned workbook can be saved by the caller, e.g. workbook.Save("result.xlsx").

```csharp
public Task<Workbook> GenerateComparisonWorkbookAsync(Workbook before, Workbook after, WorkbookComparisonOptions? options = null, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| before | Workbook | The original workbook. |
| after | Workbook | The modified workbook. |
| options | WorkbookComparisonOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a Workbook.

### See Also

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
