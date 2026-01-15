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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StylePropertyParentStyleDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Get the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data
            worksheet.Cells["A1"].Value = "Parent Style Example";
            worksheet.Cells["A2"].Value = "Child Style Example";

            try
            {
                // Create a parent style
                Style parentStyle = workbook.CreateStyle();
                parentStyle.Font.Name = "Arial";
                parentStyle.Font.Size = 12;
                parentStyle.ForegroundColor = System.Drawing.Color.LightBlue;
                parentStyle.Pattern = BackgroundType.Solid;

                // Create a child style based on the parent style
                Style childStyle = workbook.CreateStyle();
                childStyle.Font.IsBold = true;
                childStyle.Font.Color = System.Drawing.Color.Red;

                // Apply styles to cells
                Cell parentCell = worksheet.Cells["A1"];
                parentCell.SetStyle(parentStyle);

                Cell childCell = worksheet.Cells["A2"];
                childCell.SetStyle(childStyle);

                // Demonstrate ParentStyle property (read-only)
                Style retrievedChildStyle = childCell.GetStyle();
                Console.WriteLine("Child style has parent style: " +
                    (retrievedChildStyle.ParentStyle != null));

                if (retrievedChildStyle.ParentStyle != null)
                {
                    Console.WriteLine("Parent style font name: " +
                        retrievedChildStyle.ParentStyle.Font.Name);
                    Console.WriteLine("Parent style font size: " +
                        retrievedChildStyle.ParentStyle.Font.Size);
                }

                // Save the workbook
                workbook.Save("ParentStyleDemo.xlsx");
                Console.WriteLine("ParentStyle demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


