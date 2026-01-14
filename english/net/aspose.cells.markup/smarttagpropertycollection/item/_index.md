---
title: SmartTagPropertyCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: SmartTagPropertyCollection property. Gets a SmartTagProperty object
type: docs
url: /net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Gets a [`SmartTagProperty`](../../smarttagproperty/) object.

```csharp
public SmartTagProperty this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Return Value

Returns a [`SmartTagProperty`](../../smarttagproperty/) object.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create a smart tag property collection
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Add properties to the collection
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Access properties using Item indexer
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Display current property values
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Note: The Item property is read-only, so we can't assign to it directly
            // Instead, we can modify the properties of the returned SmartTagProperty objects
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Display updated values
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Save the workbook (though smart tags aren't visibly stored in a simple save)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### See Also

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Gets a [`SmartTagProperty`](../../smarttagproperty/) object by the name of the property.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the property. |

### Return Value

Returns a [`SmartTagProperty`](../../smarttagproperty/) object.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Create a smart tag setting and add a smart tag
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Get the smart tag and its properties
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Add some properties to demonstrate the Item property
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Access properties using the Item indexer (by index)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Display the property values
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Save the workbook
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
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

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


