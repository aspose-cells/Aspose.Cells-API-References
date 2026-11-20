---
title: Enum CellsAIErrorCode
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAIErrorCode enum. Stable product error codes for Cells AI operations."
type: docs
url: /net/aspose.cells.ai/cellsaierrorcode/
---
## CellsAIErrorCode enumeration

Stable product error codes for Cells AI operations.

```csharp
public enum CellsAIErrorCode
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| InvalidLocation | `0` | The location is syntactically valid but does not exist in the current workbook, belongs to another workbook, or has a mismatched type. |
| ContentAccessDenied | `1` | The operation requires unauthorized scope or hidden content that is not allowed. |
| ContentTooLarge | `2` | The content exceeds product or provider capacity limits. |
| InvalidModelOutput | `3` | The model output does not conform to the Cells AI internal structured protocol or does not pass local validation. |
| UnsupportedCapability | `4` | The provider, model or v1 product scope does not support the capability required to complete the operation. |
| ProviderFailure | `5` | A timeout, network error, authentication failure, rate limit, provider service error or other provider call failure. |
| AmbiguousRequest | `6` | The routed request could not be classified to a single operation with confidence and the caller requested a hard failure. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
