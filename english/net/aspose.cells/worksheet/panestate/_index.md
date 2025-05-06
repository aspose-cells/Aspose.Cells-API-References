---
title: Worksheet.PaneState
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the pane has horizontal or vertical splits and whether those splits are frozen
type: docs
url: /net/aspose.cells/worksheet/panestate/
---
## Worksheet.PaneState property

Indicates whether the pane has horizontal or vertical splits, and whether those splits are frozen.

```csharp
public PaneStateType PaneState { get; }
```

### Examples

```csharp
// Called: PaneStateType paneState = worksheet.PaneState;
public static void Property_PaneState()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Add a new worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Set some sample data in the worksheet
            worksheet.Cells[&quot;A1&quot;].PutValue(&quot;Data 1&quot;);
            worksheet.Cells[&quot;A2&quot;].PutValue(&quot;Data 2&quot;);
            worksheet.Cells[&quot;A3&quot;].PutValue(&quot;Data 3&quot;);
            worksheet.Cells[&quot;B1&quot;].PutValue(10);
            worksheet.Cells[&quot;B2&quot;].PutValue(20);
            worksheet.Cells[&quot;B3&quot;].PutValue(30);

            // Freeze panes at cell B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Check the pane state
            PaneStateType paneState = worksheet.PaneState;

            // Output the pane state
            Console.WriteLine(&quot;Current Pane State: &quot; + paneState);

            // Save the workbook
            workbook.Save(&quot;PaneStateTypeExample.xlsx&quot;);
        }
```

### See Also

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


