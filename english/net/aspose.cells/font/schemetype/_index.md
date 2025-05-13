---
title: Font.SchemeType
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the scheme type of the font
type: docs
url: /net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Gets and sets the scheme type of the font.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Examples

```csharp
// Called: font.SchemeType = FontSchemeType.Major;
public static void Font_Property_SchemeType()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            // Obtain the reference of the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            // Accessing the "A1" cell from the worksheet
            Cell cell = worksheet.Cells["A1"];
            // Adding some value to the "A1" cell
            cell.PutValue("Hello Aspose!");

            // Access the font of the cell style
            Aspose.Cells.Font font = cell.GetStyle().Font;

            // Setting the font scheme type to Major
            font.SchemeType = FontSchemeType.Major;

            // Setting other font properties for demonstration
            font.Name = "Arial";
            font.Size = 14;
            font.Color = System.Drawing.Color.Blue;

            // Save the workbook
            workbook.Save("FontSchemeTypeExample.xlsx");
            workbook.Save("FontSchemeTypeExample.pdf");
            return;
        }
```

### See Also

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


