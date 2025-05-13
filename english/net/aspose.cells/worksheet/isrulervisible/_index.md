---
title: Worksheet.IsRulerVisible
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Indicates whether the ruler is visible. This property is only applied for page break preview
type: docs
url: /net/aspose.cells/worksheet/isrulervisible/
---
## Worksheet.IsRulerVisible property

Indicates whether the ruler is visible. This property is only applied for page break preview.

```csharp
public bool IsRulerVisible { get; set; }
```

### Examples

```csharp
// Called: worksheet.IsRulerVisible = true;
public static void Worksheet_Property_IsRulerVisible()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Set worksheet properties
            worksheet.Name = "DemoSheet";
            worksheet.IsGridlinesVisible = true;
            worksheet.IsRowColumnHeadersVisible = true;
            worksheet.DisplayZeros = true;
            worksheet.DisplayRightToLeft = false;
            worksheet.IsOutlineShown = true;
            worksheet.IsSelected = true;
            worksheet.FirstVisibleRow = 0;
            worksheet.FirstVisibleColumn = 0;
            worksheet.Zoom = 100;
            worksheet.ViewType = ViewType.PageLayoutView;
            worksheet.IsPageBreakPreview = false;
            worksheet.IsRulerVisible = true;
            worksheet.TabColor = System.Drawing.Color.Blue;
            worksheet.CodeName = "Sheet1";
            worksheet.ActiveCell = "A1";

            // Add a hyperlink in Cell A1
            worksheet.Hyperlinks.Add("A1", 1, 1, "http://www.aspose.com");

            // Freeze panes at "C3" with 3 row and 3 column
            worksheet.FreezePanes("C3", 3, 3);

            // Add a conditional formatting rule
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            int conditionIndex = fcs.AddCondition(FormatConditionType.AboveAverage);
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // Setting properties for AboveAverage rule
            fc.AboveAverage.IsAboveAverage = true;
            fc.AboveAverage.IsEqualAverage = false;
            fc.AboveAverage.StdDev = 2;

            // Save the workbook
            workbook.Save("WorksheetExample.xlsx");

            return;
        }
```

### See Also

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


