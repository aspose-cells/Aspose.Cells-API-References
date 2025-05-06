---
title: ConditionalFormattingIcon.Type
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon property. Gets and sets the icon set type
type: docs
url: /net/aspose.cells/conditionalformattingicon/type/
---
## ConditionalFormattingIcon.Type property

Gets and sets the icon set type.

```csharp
public IconSetType Type { get; set; }
```

### Examples

```csharp
// Called: cfIcon2.Type = IconSetType.Boxes5;
public static void Property_Type()
        {
            // Instantiating a Workbook object
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Get Conditional Formatting
            ConditionalFormattingCollection cformattings = sheet.ConditionalFormattings;

            // Adds an empty conditional formatting
            int index = cformattings.Add();

            // Get newly added Conditional formatting
            FormatConditionCollection fcs = cformattings[index];

            // Sets the conditional format range.
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            ca = new CellArea
            {
                StartRow = 1,
                EndRow = 1,
                StartColumn = 1,
                EndColumn = 1
            };
            fcs.AddArea(ca);

            // Sets condition
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // Sets condition&apos;s type
            cond.IconSet.Type = IconSetType.ArrowsGray3;

            // Add custom iconset condition.
            ConditionalFormattingIcon cfIcon = cond.IconSet.CfIcons[0];
            cfIcon.Type = IconSetType.Arrows3;
            cfIcon.Index = 0;

            ConditionalFormattingIcon cfIcon1 = cond.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Saving the Excel file
            workbook.Save(&quot;outConditionalFormattingIconCollectionDemoput.xlsx&quot;);
            workbook.Save(&quot;outConditionalFormattingIconCollectionDemoput.pdf&quot;);
        }
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


