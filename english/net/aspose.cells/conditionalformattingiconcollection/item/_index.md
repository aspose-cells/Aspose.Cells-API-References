---
title: ConditionalFormattingIconCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIconCollection property. Gets the ConditionalFormattingIcon element at the specified index
type: docs
url: /net/aspose.cells/conditionalformattingiconcollection/item/
---
## ConditionalFormattingIconCollection indexer

Gets the ConditionalFormattingIcon element at the specified index.

```csharp
public ConditionalFormattingIcon this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |

### Return Value

The element at the specified index.

### Examples

```csharp
// Called: ConditionalFormattingIcon cfIcon2 = cond.IconSet.CfIcons[2];
public static void ConditionalFormattingIconCollection_Property_Item()
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

            // Sets condition's type
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
            workbook.Save("outConditionalFormattingIconCollectionDemoput.xlsx");
            workbook.Save("outConditionalFormattingIconCollectionDemoput.pdf");
        }
```

### See Also

* class [ConditionalFormattingIcon](../../conditionalformattingicon/)
* class [ConditionalFormattingIconCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


