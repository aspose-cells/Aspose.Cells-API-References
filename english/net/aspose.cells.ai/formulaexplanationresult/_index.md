---
title: Class FormulaExplanationResult
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.FormulaExplanationResult class. The result of ExplainFormulaAsync."
type: docs
url: /net/aspose.cells.ai/formulaexplanationresult/
---
## FormulaExplanationResult class

The result of ExplainFormulaAsync.

```csharp
public sealed class FormulaExplanationResult : CellsAIResult
```

## Properties

| Name | Description |
| --- | --- |
| [Dependencies](dependencies/) { get; } | The locally validated dependencies of the formula. Never null. |
| [Explanation](explanation/) { get; } | The natural language explanation. |
| [Formula](formula/) { get; } | The formula that was explained. |
| [Operation](operation/) { get; } | Gets the operation that produced this result. |
| [Text](text/) { get; } | Gets the human-readable representation of the result. |

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
