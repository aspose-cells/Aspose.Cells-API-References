---
title: IconSet.Type
second_title: Aspose.Cells for .NET API Reference
description: IconSet property. Get or Set the icon set type to display. Setting the type will auto check if the current Cfvoss count is accord with the new type. If not accord old Cfvos will be cleaned and default Cfvos will be added
type: docs
url: /net/aspose.cells/iconset/type/
---
## IconSet.Type property

Get or Set the icon set type to display. Setting the type will auto check if the current Cfvos's count is accord with the new type. If not accord, old Cfvos will be cleaned and default Cfvos will be added.

```csharp
public IconSetType Type { get; set; }
```

### Examples

```csharp
// Called: iconSet.Type = IconSetType.Arrows3;
public static void Property_Type()
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
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // Saving the Excel file
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
```

### See Also

* enum [IconSetType](../../iconsettype/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


