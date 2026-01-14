---
title: Class SmartTagProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markup.SmartTagProperty class. Represents the property of the cell smart tag
type: docs
url: /net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Represents the property of the cell smart tag.

```csharp
public class SmartTagProperty
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Gets and sets the name of the property. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Gets and sets the value of the property. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Create an instance of SmartTagProperty using reflection since constructor is non-public
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Set the Name and Value properties
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Display the property values
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Demonstrate modifying the properties
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


