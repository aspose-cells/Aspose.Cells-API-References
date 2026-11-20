---
title: Aspose.Cells.AI
second_title: Aspose.Cells for .NET API Reference
description: "The Aspose.Cells.AI namespace provides provider-neutral, AI-powered workbook capabilities: summarization, Q&A, inspection, formula explanation and generation, workbook editing and workbook comparison. A single reusable CellsAI instance backs all business methods; Aspose.Cells performs all local validation and editing."
type: docs
url: /net/aspose.cells.ai/
---
The Aspose.Cells.AI namespace provides provider-neutral, AI-powered workbook capabilities: summarization, Q&A, inspection, formula explanation and generation, workbook editing and workbook comparison. A single reusable CellsAI instance backs all business methods; Aspose.Cells performs all local validation and editing.

## Classes

| Class | Description |
| --- | --- |
| [CellsAI](cellsai/) | The application-level entry point for Cells AI. Reusable, thread-safe for concurrent calls against unrelated workbooks, and carries no business session state. |
| [CellsAIBuilder](cellsaibuilder/) | Fluent creation of a CellsAI instance. Each builder configures exactly one provider and Build can only succeed once. |
| [CellsAIException](cellsaiexception/) | The exception thrown when a Cells AI operation fails. Provider raw exceptions are never exposed as InnerException. |
| [CellsAIResult](cellsairesult/) | The base class of all Cells AI operation results. Instances are immutable objects with no public constructors. |
| [CellsAIUsage](cellsaiusage/) | Usage information for a single operation. |
| [CellsAIWarning](cellsaiwarning/) | A non-fatal warning returned with a result. Code is a stable, machine-usable identifier, not free text. |
| [FormulaExplanationResult](formulaexplanationresult/) | The result of ExplainFormulaAsync. |
| [FormulaGenerationResult](formulagenerationresult/) | The result of GenerateFormulaAsync. |
| [WorkbookAnswerResult](workbookanswerresult/) | The result of AskAsync. |
| [WorkbookChange](workbookchange/) | A change applied to a workbook by EditAsync. |
| [WorkbookCitation](workbookcitation/) | A reference to a location in the workbook that backs a statement in a result. Citations are locally validated to point to an existing and authorized location. |
| [WorkbookComparisonOptions](workbookcomparisonoptions/) | Controls the scope of CompareAsync. |
| [WorkbookComparisonResult](workbookcomparisonresult/) | The result of CompareAsync. |
| [WorkbookContentOptions](workbookcontentoptions/) | Controls which workbook content is readable by the model for content producing operations such as SummarizeAsync, AskAsync, ExplainFormulaAsync and GenerateFormulaAsync. |
| [WorkbookDifference](workbookdifference/) | A difference between two workbooks produced by CompareAsync. For added content BeforeLocation is null; for removed content AfterLocation is null. |
| [WorkbookEditOptions](workbookeditoptions/) | The write scope for EditAsync. WritableLocations is the write safety boundary; ContextLocations is readable only. |
| [WorkbookEditResult](workbookeditresult/) | The result of EditAsync. It owns UpdatedWorkbook; disposing the result also disposes the updated workbook. |
| [WorkbookFinding](workbookfinding/) | A finding produced by InspectAsync. Code is a stable, machine-usable identifier, not free text. |
| [WorkbookInspectionOptions](workbookinspectionoptions/) | Controls the scope of InspectAsync. |
| [WorkbookInspectionResult](workbookinspectionresult/) | The result of InspectAsync. |
| [WorkbookLocation](workbooklocation/) | A structured value object that identifies a part of a workbook: a worksheet, a cell, a range, a ListObject (table) or a defined name. |
| [WorkbookRouterOptions](workbookrouteroptions/) | Controls how ProcessAsync routes a natural-language request to a single operation. Safety boundaries are not relaxed: the model never chooses writable locations or content scope on its own. |
| [WorkbookSummaryResult](workbooksummaryresult/) | The result of SummarizeAsync. |

## Enumerations

| Enumeration | Description |
| --- | --- |
| [CellsAIContentLimitKind](cellsaicontentlimitkind/) | The capacity limit that was exceeded when a CellsAIException with ContentTooLarge is thrown. |
| [CellsAIErrorCode](cellsaierrorcode/) | Stable product error codes for Cells AI operations. |
| [WorkbookChangeKind](workbookchangekind/) | The kind of a WorkbookChange produced by EditAsync. |
| [WorkbookComparisonDimension](workbookcomparisondimension/) | The dimensions compared by CompareAsync. |
| [WorkbookDifferenceKind](workbookdifferencekind/) | The kind of a WorkbookDifference produced by CompareAsync. |
| [WorkbookFindingSeverity](workbookfindingseverity/) | The severity of a WorkbookFinding. |
| [WorkbookInspectionScope](workbookinspectionscope/) | The categories inspected by InspectAsync. |
| [WorkbookLocationKind](workbooklocationkind/) | The kind of a workbook location. |
| [WorkbookOperationKind](workbookoperationkind/) | The operations the intent router may select. Used to restrict routing scope and to name the operation chosen by ProcessAsync. |

