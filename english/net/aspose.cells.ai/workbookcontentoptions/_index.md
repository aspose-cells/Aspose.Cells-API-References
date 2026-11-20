---
title: Class WorkbookContentOptions
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookContentOptions class. Controls which workbook content is readable by the model for content producing operations such as SummarizeAsync, AskAsync, ExplainFormulaAsync and GenerateFormulaAsync."
type: docs
url: /net/aspose.cells.ai/workbookcontentoptions/
---
## WorkbookContentOptions class

Controls which workbook content is readable by the model for content producing operations such as SummarizeAsync, AskAsync, ExplainFormulaAsync and GenerateFormulaAsync.

```csharp
public sealed class WorkbookContentOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookContentOptions](workbookcontentoptions/)(WorkbookLocation[]) | Creates options for the specified locations. |

## Properties

| Name | Description |
| --- | --- |
| [IncludeHiddenContent](includehiddencontent/) { get; set; } | Whether hidden worksheets, hidden rows, hidden columns and filtered rows are allowed to be sent to the model. Default is false. |
| [Locations](locations/) { get; } | The authorized locations to read. Empty means "visible used content of the workbook". |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
