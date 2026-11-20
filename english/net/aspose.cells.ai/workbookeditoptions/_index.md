---
title: Class WorkbookEditOptions
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.WorkbookEditOptions class. The write scope for EditAsync. WritableLocations is the write safety boundary; ContextLocations is readable only."
type: docs
url: /net/aspose.cells.ai/workbookeditoptions/
---
## WorkbookEditOptions class

The write scope for EditAsync. WritableLocations is the write safety boundary; ContextLocations is readable only.

```csharp
public sealed class WorkbookEditOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [WorkbookEditOptions](workbookeditoptions/)(WorkbookLocation, WorkbookLocation[]) | Creates options with one writable location and optional additional writable locations. |

## Properties

| Name | Description |
| --- | --- |
| [ContextLocations](contextlocations/) { get; } | Additional locations the model may read but not write. Mutable, so callers can add context locations before invoking EditAsync. |
| [IncludeHiddenContent](includehiddencontent/) { get; set; } | Whether hidden content is allowed. Default is false. |
| [WritableLocations](writablelocations/) { get; } | The locations the model is allowed to write. Immutable after construction. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
