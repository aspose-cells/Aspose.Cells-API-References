---
title: SmartTag.Name
second_title: Aspose.Cells for .NET API Reference
description: SmartTag property. Gets the name of the smart tag
type: docs
url: /net/aspose.cells.markup/smarttag/name/
---
## SmartTag.Name property

Gets the name of the smart tag.

```csharp
public string Name { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples.SmartTagPropertyNameDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyNameDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            try
            {
                // Create a smart tag instance using reflection (since constructor isn't public)
                Type smartTagType = typeof(SmartTag);
                SmartTag smartTag = (SmartTag)Activator.CreateInstance(smartTagType, nonPublic: true);
                
                // Initialize the smart tag with sample values
                smartTag.SetLink("http://example.com/smarttags", "SampleSmartTag");
                
                // Demonstrate the Name property (read-only operation)
                Console.WriteLine("SmartTag Name: " + smartTag.Name);
                
                // Save the workbook
                workbook.Save("SmartTagNameDemo.xlsx");
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

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


