---
title: Class WorkbookEditResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookEditResult class. The result of EditAsync. It owns UpdatedWorkbook; disposing the result also disposes the updated workbook."
type: docs
url: /net/aspose.cells.ai/workbookeditresult/
---
## WorkbookEditResult class

The result of EditAsync. It owns UpdatedWorkbook; disposing the result also disposes the updated workbook.

```csharp
public sealed class WorkbookEditResult : CellsAIResult, IDisposable
```

## Properties

| Name | Description |
| --- | --- |
| [Changes](changes/) { get; } | The changes applied to the workbook. Never null. |
| [Operation](operation/) { get; } | Gets the operation that produced this result. |
| [Text](text/) { get; } | Gets the human-readable representation of the result. |
| [UpdatedWorkbook](updatedworkbook/) { get; } | The edited workbook. Never the input workbook. |

## Methods

| Name | Description |
| --- | --- |
| [Dispose](dispose/)() | Releases the resources used by this instance. |

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
