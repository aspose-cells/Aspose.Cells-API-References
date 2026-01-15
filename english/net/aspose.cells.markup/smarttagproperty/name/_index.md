---
title: SmartTagProperty.Name
second_title: Aspose.Cells for .NET API Reference
description: SmartTagProperty property. Gets and sets the name of the property
type: docs
url: /net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Gets and sets the name of the property.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of SmartTagProperty using reflection since constructor is non-public
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Set the Name property
                property.Name = "Department";

                // Display the current value of the Name property
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Demonstrate changing the Name property
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Show that the property can be read and modified
                Console.WriteLine("Name property demonstration completed successfully");
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

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


