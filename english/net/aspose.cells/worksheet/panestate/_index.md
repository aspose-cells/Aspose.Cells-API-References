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
            worksheet.Cells["A1"].PutValue("Data 1");
            worksheet.Cells["A2"].PutValue("Data 2");
            worksheet.Cells["A3"].PutValue("Data 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Freeze panes at cell B2
            worksheet.FreezePanes(1, 0, 1, 1); // Freeze the first row and first column

            // Check the pane state
            PaneStateType paneState = worksheet.PaneState;

            // Output the pane state
            Console.WriteLine("Current Pane State: " + paneState);

            // Save the workbook
            workbook.Save("PaneStateTypeExample.xlsx");
        }
```

### See Also

* enum [PaneStateType](../../panestatetype/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


