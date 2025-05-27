---
title: Class DocumentProperty
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Properties.DocumentProperty class. Represents a custom or builtin document property
type: docs
url: /net/aspose.cells.properties/documentproperty/
---
## DocumentProperty class

Represents a custom or built-in document property.

```csharp
public class DocumentProperty
```

## Properties

| Name | Description |
| --- | --- |
| [IsGeneratedName](../../aspose.cells.properties/documentproperty/isgeneratedname/) { get; } | Returns true if this property does not have a name in the OLE2 storage and a unique name was generated only for the public API. |
| [IsLinkedToContent](../../aspose.cells.properties/documentproperty/islinkedtocontent/) { get; } | Indicates whether this property is linked to content |
| [Name](../../aspose.cells.properties/documentproperty/name/) { get; } | Returns the name of the property. |
| [Source](../../aspose.cells.properties/documentproperty/source/) { get; } | The linked content source. |
| [Type](../../aspose.cells.properties/documentproperty/type/) { get; } | Gets the data type of the property. |
| [Value](../../aspose.cells.properties/documentproperty/value/) { get; set; } | Gets or sets the value of the property. |

## Methods

| Name | Description |
| --- | --- |
| [ToBool](../../aspose.cells.properties/documentproperty/tobool/)() | Returns the property value as bool. |
| [ToDateTime](../../aspose.cells.properties/documentproperty/todatetime/)() | Returns the property value as DateTime in local timezone. |
| [ToDouble](../../aspose.cells.properties/documentproperty/todouble/)() | Returns the property value as double. |
| [ToInt](../../aspose.cells.properties/documentproperty/toint/)() | Returns the property value as integer. |
| override [ToString](../../aspose.cells.properties/documentproperty/tostring/)() | Returns the property value as a string. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Properties;
    using System;

    public class DocumentPropertyDemo
    {
        public static void DocumentPropertyExample()
        {
            //// Instantiate a Workbook object
            //Workbook workbook = new Workbook("DocumentProperty_original.xlsx");

            //// Retrieve a list of all custom document properties of the Excel file
            //DocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;

            //// Accessing a custom document property by using the property index
            //DocumentProperty customProperty1 = customProperties[3];

            //// Accessing a custom document property by using the property name
            //DocumentProperty customProperty2 = customProperties["Owner"];

            //// Displaying properties of the custom document property
            //Console.WriteLine("Property Name: " + customProperty2.Name);
            //Console.WriteLine("Property Value: " + customProperty2.Value);
            //Console.WriteLine("Is Linked To Content: " + customProperty2.IsLinkedToContent);
            //Console.WriteLine("Source: " + customProperty2.Source);
            //Console.WriteLine("Type: " + customProperty2.Type);
            //Console.WriteLine("Is Generated Name: " + customProperty2.IsGeneratedName);

            //// Using methods to get property values in different formats
            //Console.WriteLine("Property Value as String: " + customProperty2.ToString());
            //Console.WriteLine("Property Value as Integer: " + customProperty2.ToInt());
            //Console.WriteLine("Property Value as Double: " + customProperty2.ToDouble());
            //Console.WriteLine("Property Value as DateTime: " + customProperty2.ToDateTime());
            //Console.WriteLine("Property Value as Boolean: " + customProperty2.ToBool());

            //// Setting a new value to the custom property
            //customProperty2.Value = "New Owner";

            //// Save the workbook
            //workbook.Save("DocumentPropertyExample.xlsx");
            //workbook.Save("DocumentPropertyExample.pdf");
            return;
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Properties](../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../)


