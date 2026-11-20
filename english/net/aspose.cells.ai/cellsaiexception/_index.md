---
title: Class CellsAIException
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAIException class. The exception thrown when a Cells AI operation fails. Provider raw exceptions are never exposed as InnerException."
type: docs
url: /net/aspose.cells.ai/cellsaiexception/
---
## CellsAIException class

The exception thrown when a Cells AI operation fails. Provider raw exceptions are never exposed as InnerException.

```csharp
public sealed class CellsAIException : Exception
```

## Constructors

| Name | Description |
| --- | --- |
| [CellsAIException](cellsaiexception/)(CellsAIErrorCode, String) | Creates an exception with a stable error code and message. |

## Properties

| Name | Description |
| --- | --- |
| [ContentLimitKind](contentlimitkind/) { get; } | Only populated when ErrorCode is ContentTooLarge. It does not contain workbook content. |
| [DiagnosticId](diagnosticid/) { get; } | An identifier used to correlate with controlled internal diagnostics. It does not contain workbook content, provider responses or credentials. |
| [ErrorCode](errorcode/) { get; } | The stable error code. |
| [LimitValue](limitvalue/) { get; } | The configured limit value. Only for ContentTooLarge. |
| [ObservedValue](observedvalue/) { get; } | The observed value that exceeded the limit. Only for ContentTooLarge. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
