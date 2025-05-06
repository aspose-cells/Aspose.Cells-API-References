---
title: Enum IconSetType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.IconSetType enum. Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable and the icon order is reversible
type: docs
url: /net/aspose.cells/iconsettype/
---
## IconSetType enumeration

Icon set type for conditional formatting. The threshold values for triggering the different icons within a set are configurable, and the icon order is reversible.

```csharp
public enum IconSetType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| Arrows3 | `0` | 3 arrows icon set. |
| ArrowsGray3 | `1` | 3 gray arrows icon set. |
| Flags3 | `2` | 3 flags icon set. |
| Signs3 | `3` | 3 signs icon set. |
| Symbols3 | `4` | 3 symbols icon set (circled). |
| Symbols32 | `5` | 3 Symbols icon set (uncircled). |
| TrafficLights31 | `6` | 3 traffic lights icon set (unrimmed). |
| TrafficLights32 | `7` | 3 traffic lights icon set with thick black border. |
| Arrows4 | `8` | 4 arrows icon set. |
| ArrowsGray4 | `9` | 4 gray arrows icon set. |
| Rating4 | `10` | 4 ratings icon set. |
| RedToBlack4 | `11` | 4 'red to black' icon set. |
| TrafficLights4 | `12` | 4 traffic lights icon set. |
| Arrows5 | `13` | 5 arrows icon set. |
| ArrowsGray5 | `14` | 5 gray arrows icon set. |
| Quarters5 | `15` | 5 quarters icon set. |
| Rating5 | `16` | 5 rating icon set. |
| Stars3 | `17` | 3 stars set |
| Boxes5 | `18` | 5 boxes set |
| Triangles3 | `19` | 3 triangles set |
| None | `20` | None |
| CustomSet | `21` | CustomSet. This element is read-only. |
| Smilies3 | `22` | 3 smilies. Only for .ods. |
| ColorSmilies3 | `23` | 3 color smilies. Only for .ods. |

### Examples

```csharp
// Called: cfIcon1.Type = IconSetType.ArrowsGray3;
public static void Type_IconSetType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access the first worksheet in the workbook
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Get the Conditional Formattings Collection
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // Add a new conditional formatting to the collection
            int index = cformattings.Add();
            
            // Access the Format Condition Collection
            FormatConditionCollection fcs = cformattings[index];
            
            // Define the cell area to apply conditional formatting
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // Add the cell area to the format condition collection
            fcs.AddArea(ca);
            
            // Add a condition to use icon sets
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // Set the icon set type
            fc.IconSet.Type = IconSetType.Arrows3;

            // Customize the individual icons within the icon set
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // Save the workbook
            workbook.Save(&quot;ConditionalFormattingIconExample.xlsx&quot;);
            workbook.Save(&quot;ConditionalFormattingIconExample.pdf&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


