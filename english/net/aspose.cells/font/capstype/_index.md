---
title: Font.CapsType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the text caps type
type: docs
url: /net/aspose.cells/font/capstype/
---
## Font.CapsType property

Gets and sets the text caps type.

```csharp
public TextCapsType CapsType { get; set; }
```

### Examples

```csharp
// Called: style.Font.CapsType = Aspose.Cells.TextCapsType.All;
public static void Property_CapsType()
        {
            // Additional code to demonstrate how the instance might be used
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set a cell's value
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Hello Aspose!");

            // Get the cell's style
            Style style = cell.GetStyle();

            // Set the font caps type to All Caps
            style.Font.CapsType = Aspose.Cells.TextCapsType.All;

            // Apply the style to the cell
            cell.SetStyle(style);

            // Save the workbook
            workbook.Save("TextCapsTypeExample.xlsx");

            return;
        }
```

### See Also

* enum [TextCapsType](../../textcapstype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


