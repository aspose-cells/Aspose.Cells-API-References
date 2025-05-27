---
title: SmartTag.Deleted
second_title: Aspose.Cells for .NET API Reference
description: SmartTag property. Indicates whether the smart tag is deleted
type: docs
url: /net/aspose.cells.markup/smarttag/deleted/
---
## SmartTag.Deleted property

Indicates whether the smart tag is deleted.

```csharp
public bool Deleted { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyDeletedDemo
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
                
                // Demonstrate the Deleted property (read/write operation)
                Console.WriteLine("Initial Deleted value: " + smartTag.Deleted);
                
                // Set the Deleted property to true
                smartTag.Deleted = true;
                Console.WriteLine("After setting Deleted: " + smartTag.Deleted);
                
                // Save the workbook
                workbook.Save("SmartTagDeletedDemo.xlsx");
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


