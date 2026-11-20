---
title: Class WorkbookRouterOptions
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookRouterOptions class. Controls how ProcessAsync routes a natural-language request to a single operation. Safety boundaries are not relaxed: the model never chooses writable locations or content scope on its own."
type: docs
url: /net/aspose.cells.ai/workbookrouteroptions/
---
## WorkbookRouterOptions class

Controls how ProcessAsync routes a natural-language request to a single operation. Safety boundaries are not relaxed: the model never chooses writable locations or content scope on its own.

```csharp
public sealed class WorkbookRouterOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookRouterOptions](workbookrouteroptions/)() | Initializes a new instance of the WorkbookRouterOptions class. |

## Properties

| Name | Description |
| --- | --- |
| [AllowedOperations](allowedoperations/) { get; set; } | The operations the router may select, or null for all. Requests classified outside this set are treated as ambiguous. |
| [ContextLocations](contextlocations/) { get; } | Additional locations the model may read but not write. For edit requests these become the edit context; for read operations they restrict the readable scope. Empty means "the visible used content of the workbook". |
| [FailOnAmbiguous](failonambiguous/) { get; set; } | When true, a request that cannot be classified with confidence throws AmbiguousRequest instead of failing over to Ask. Default is false. |
| [IncludeHiddenContent](includehiddencontent/) { get; set; } | Whether hidden worksheets, hidden rows, hidden columns and filtered rows are allowed to be disclosed to the model. Default is false. |
| [WritableLocations](writablelocations/) { get; } | The locations the model is allowed to write. Only required when the request is routed to Edit; passed through to the edit operation as its write safety boundary. The model never decides these. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
