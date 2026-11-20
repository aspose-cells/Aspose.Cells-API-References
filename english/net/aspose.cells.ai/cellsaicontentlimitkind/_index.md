---
title: Enum CellsAIContentLimitKind
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAIContentLimitKind enum. The capacity limit that was exceeded when a CellsAIException with ContentTooLarge is thrown."
type: docs
url: /net/aspose.cells.ai/cellsaicontentlimitkind/
---
## CellsAIContentLimitKind enumeration

The capacity limit that was exceeded when a CellsAIException with ContentTooLarge is thrown.

```csharp
public enum CellsAIContentLimitKind
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| NonEmptyCellCount | `0` | The number of non-empty cells exceeds the limit. |
| FieldUtf8Bytes | `1` | A single field (value, formula, comment, ...) exceeds the UTF-8 byte limit. |
| SerializedUtf8Bytes | `2` | The serialized content to send exceeds the UTF-8 byte limit. |
| InputTokens | `3` | The workbook content input token budget is exceeded. |
| OutputTokens | `4` | The reserved output tokens cannot be accommodated. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
