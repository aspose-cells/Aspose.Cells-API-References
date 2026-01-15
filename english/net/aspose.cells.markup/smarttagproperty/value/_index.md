---
title: SmartTagProperty.Value
second_title: Aspose.Cells for .NET API Reference
description: SmartTagProperty property. Gets and sets the value of the property
type: docs
url: /net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Gets and sets the value of the property.

```csharp
public string Value { get; set; }
```

### Examples

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of SmartTagProperty using the non‑public constructor
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Set the name and value of the property
                property.Name = "Category";
                property.Value = "Finance";

                // Display the property values
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
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


