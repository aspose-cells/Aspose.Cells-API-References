---
title: HighlightChangesOptions.HighlightChangesOptions
second_title: Aspose.Cells for .NET API Reference
description: HighlightChangesOptions constructor. Represents options of highlighting revsions or changes of shared Excel files
type: docs
url: /net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Represents options of highlighting revsions or changes of shared Excel files.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parameter | Type | Description |
| --- | --- | --- |
| highlightOnScreen | Boolean | Indicates whether highlighting changes on screen. |
| listOnNewSheet | Boolean | Indicates whether listing changes on a new worksheet. |

### Examples

```csharp
// Called: HighlightChangesOptions options = new HighlightChangesOptions(true, true);
public static void HighlightChangesOptions_Constructor()
        {
            // Instantiate a Workbook object
            Workbook workbook = new Workbook("HighlightedChangesWorkbook_original.xlsx");

            // Get the revision logs
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Set the number of days to preserve the history
            revisionLogs.DaysPreservingHistory = 30;

            // Create HighlightChangesOptions
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);

            // Highlight changes
            revisionLogs.HighlightChanges(options);

            // Save the workbook with highlighted changes
            workbook.Save("HighlightedChangesWorkbook.xlsx");
            workbook.Save("HighlightedChangesWorkbook.pdf");
        }
```

### See Also

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


