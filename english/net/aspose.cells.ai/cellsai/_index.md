---
title: Class CellsAI
second_title: Aspose.Cells for .NET API Reference
description: "Aspose.Cells.AI.CellsAI class. The application-level entry point for Cells AI. Reusable, thread-safe for concurrent calls against unrelated workbooks, and carries no business session state."
type: docs
url: /net/aspose.cells.ai/cellsai/
---
## CellsAI class

The application-level entry point for Cells AI. Reusable, thread-safe for concurrent calls against unrelated workbooks, and carries no business session state.

```csharp
public sealed class CellsAI : IDisposable
```

## Constructors

| Name | Description |
| --- | --- |
| [CellsAI](cellsai/)(IChatClient) | Creates a Cells AI instance that borrows an existing chat client. The caller keeps ownership of chatClient and is responsible for disposing it. |

## Methods

| Name | Description |
| --- | --- |
| [AskAsync](askasync/)(Workbook, String, WorkbookContentOptions, CancellationToken) | Answers a question about a workbook, with supporting citations. |
| [CompareAsync](compareasync/)(Workbook, Workbook, WorkbookComparisonOptions, CancellationToken) | Compares two workbooks and summarizes the differences. |
| static [CreateAnthropic](createanthropic/)(String, String, Uri) | Creates a Cells AI instance backed by the Anthropic Messages endpoint. |
| static [CreateBuilder](createbuilder/)() | Returns a fluent builder for creating a Cells AI instance. |
| static [CreateOpenAI](createopenai/)(String, String, Uri) | Creates a Cells AI instance backed by an OpenAI-compatible chat completion endpoint. |
| [Dispose](dispose/)() | Releases the resources used by this instance. |
| [EditAsync](editasync/)(Workbook, String, WorkbookEditOptions, CancellationToken) | Edits a copy of the workbook according to instructions and returns the new workbook. The input workbook is never modified. |
| [ExplainFormulaAsync](explainformulaasync/)(Cell, WorkbookContentOptions, CancellationToken) | Explains an existing formula in plain language. |
| [GenerateComparisonWorkbookAsync](generatecomparisonworkbookasync/)(Workbook, Workbook, WorkbookComparisonOptions, CancellationToken) | Compares two workbooks and produces a marked-up workbook that visualizes the differences the way document comparison tools do: inserted content is blue, deleted content is red, and cells whose value is unchanged but whose formatting differs are green. A changed cell shows the new value followed by the old value inside the same cell. The returned workbook can be saved by the caller, e.g. workbook.Save("result.xlsx"). |
| [GenerateFormulaAsync](generateformulaasync/)(Cell, String, WorkbookContentOptions, CancellationToken) | Generates a formula for a target cell that passes the Aspose.Cells parser and calculation engine validation. The input workbook is not modified. |
| [InspectAsync](inspectasync/)(Workbook, WorkbookInspectionOptions, CancellationToken) | Inspects a workbook for formula, data and structure issues. |
| [ProcessAsync](processasync/#processasync)(IReadOnlyList<Workbook>, String, WorkbookRouterOptions, CancellationToken) | Routes a natural-language request against one or more workbooks. Pass exactly two workbooks to enable comparison requests; a single workbook covers all other operations. Requests that combine or chain operations are not supported in a single call and fail over to an informational answer unless FailOnAmbiguous is set. |
| [ProcessAsync](processasync/#processasync_1)(Workbook, String, WorkbookRouterOptions, CancellationToken) | Routes a natural-language request to a single operation: summarize, ask, inspect, explain or generate a formula, edit, or compare. The caller never chooses the operation; the router classifies the intent in the context of workbook and dispatches to the existing operation. Safety boundaries are not relaxed - for example an edit request still requires writable locations - and the return type is the concrete result of whichever operation ran. |
| [SummarizeAsync](summarizeasync/)(Workbook, WorkbookContentOptions, CancellationToken) | Summarizes a workbook into a summary, key points and citations. |

### See Also

* namespace [Aspose.Cells.AI](../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../)
