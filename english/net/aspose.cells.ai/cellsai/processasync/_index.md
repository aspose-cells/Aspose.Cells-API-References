---
title: CellsAI.ProcessAsync
second_title: Aspose.Cells for .NET API Reference
description: "CellsAI method. Routes a natural-language request against one or more workbooks. Pass exactly two workbooks to enable comparison requests; a single workbook covers all other operations. Requests that combine or chain operations are not supported in a single call and fail over to an informational answer unless FailOnAmbiguous is set."
type: docs
url: /net/aspose.cells.ai/cellsai/processasync/
---
## CellsAI.ProcessAsync(IReadOnlyList<Workbook>, String, WorkbookRouterOptions, CancellationToken) {#processasync}

Routes a natural-language request against one or more workbooks. Pass exactly two workbooks to enable comparison requests; a single workbook covers all other operations. Requests that combine or chain operations are not supported in a single call and fail over to an informational answer unless FailOnAmbiguous is set.

```csharp
public Task<CellsAIResult> ProcessAsync(IReadOnlyList<Workbook> workbooks, string request, WorkbookRouterOptions? options = null, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbooks | IReadOnlyList<Workbook> | The workbooks to process. |
| request | String | The natural-language request. |
| options | WorkbookRouterOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a CellsAIResult.

---

## CellsAI.ProcessAsync(Workbook, String, WorkbookRouterOptions, CancellationToken) {#processasync_1}

Routes a natural-language request to a single operation: summarize, ask, inspect, explain or generate a formula, edit, or compare. The caller never chooses the operation; the router classifies the intent in the context of workbook and dispatches to the existing operation. Safety boundaries are not relaxed - for example an edit request still requires writable locations - and the return type is the concrete result of whichever operation ran.

```csharp
public Task<CellsAIResult> ProcessAsync(Workbook workbook, string request, WorkbookRouterOptions? options = null, CancellationToken cancellationToken = default)
```

| Parameter | Type | Description |
| --- | --- | --- |
| workbook | Workbook | The workbook to process. |
| request | String | The natural-language request. |
| options | WorkbookRouterOptions | The options that control the operation, or null to use the defaults. |
| cancellationToken | CancellationToken | A token that can be used to cancel the operation. |

### Return Value

A task whose result is a CellsAIResult.

### See Also

* class [CellsAI](../)
* namespace [Aspose.Cells.AI](../../../aspose.cells.ai/)
* assembly [Aspose.Cells.AI](../../../)
