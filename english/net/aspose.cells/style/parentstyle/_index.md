---
title: Style.ParentStyle
second_title: Aspose.Cells for .NET API Reference
description: Style property. Gets the parent style of this style
type: docs
url: /net/aspose.cells/style/parentstyle/
---
## Style.ParentStyle property

Gets the parent style of this style.

```csharp
public Style ParentStyle { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a base style
            Style baseStyle = workbook.CreateStyle();
            baseStyle.Name = "BaseStyle";
            baseStyle.Font.Size = 12;
            baseStyle.Font.IsBold = true;

            // Create a child style
            Style childStyle = workbook.CreateStyle();
            // Set parent style through Copy method
            childStyle.Copy(baseStyle);
            childStyle.Font.Size = 14; // Override just the font size

            // Apply the child style to a cell
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(childStyle);

            // Demonstrate ParentStyle functionality
            Console.WriteLine("Cell style font size: " + cell.GetStyle().Font.Size); // Output: 14
            Console.WriteLine("Parent style name: " + baseStyle.Name); // Output: BaseStyle
            Console.WriteLine("Parent style font size: " + baseStyle.Font.Size); // Output: 12
            Console.WriteLine("Parent style bold: " + baseStyle.Font.IsBold); // Output: True

            // Save the workbook
            workbook.Save("output.xlsx");
        }
    }
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


