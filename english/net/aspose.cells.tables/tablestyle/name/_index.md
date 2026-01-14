---
title: TableStyle.Name
second_title: Aspose.Cells for .NET API Reference
description: TableStyle property. Gets the name of table style
type: docs
url: /net/aspose.cells.tables/tablestyle/name/
---
## TableStyle.Name property

Gets the name of table style.

```csharp
public string Name { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStylePropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the table styles collection
            TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;

            try
            {
                // Get the first table style from the collection
                TableStyle tableStyle = tableStyles[0];

                // Display the Name property value
                Console.WriteLine("Table Style Name: " + tableStyle.Name);

                // Demonstrate accessing the read-only property
                string styleName = tableStyle.Name;
                Console.WriteLine("Retrieved style name: " + styleName);

                // Show that we can use the name to reference the style
                Console.WriteLine("This table style can be referenced by name: " + tableStyle.Name);

                // Save the workbook
                workbook.Save("TableStyleNameDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [TableStyle](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


