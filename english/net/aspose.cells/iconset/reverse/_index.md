---
title: IconSet.Reverse
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false
type: docs
url: /net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

Get or set the flag indicating whether to reverses the default order of the icons in this icon set. Default value is false.

```csharp
public bool Reverse { get; set; }
```

### Examples

```csharp
// Called: iconSet.Reverse = false;
public static void Property_Reverse()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Adds an empty conditional formatting
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // Sets the conditional format range
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // Adds condition
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Get Icon Set
            IconSet iconSet = cond.IconSet;

            // Set Icon Type
            iconSet.Type = IconSetType.Arrows3;

            // Set additional properties
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // Put Cell Values
            sheet.Cells[&quot;A1&quot;].PutValue(10);
            sheet.Cells[&quot;A2&quot;].PutValue(120);
            sheet.Cells[&quot;A3&quot;].PutValue(260);

            // Saving the Excel file
            workbook.Save(&quot;IconSetExample.xlsx&quot;);
            workbook.Save(&quot;IconSetExample.pdf&quot;);
        }
```

### See Also

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


