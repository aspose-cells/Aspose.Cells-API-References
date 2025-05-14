---
title: ICustomParser.ParseObject
second_title: Aspose.Cells for .NET API Reference
description: ICustomParser method. Parses given string to proper value object
type: docs
url: /net/aspose.cells/icustomparser/parseobject/
---
## ICustomParser.ParseObject method

Parses given string to proper value object.

```csharp
public object ParseObject(string value)
```

| Parameter | Type | Description |
| --- | --- | --- |
| value | String | The string value to be parsed |

### Return Value

Parsed value object from given string. If given string cannot be parsed to proper value object, returns null.

### Examples

```csharp
// Called: object parsedValue = customParser.ParseObject(valueToParse);
public static void ICustomParser_Method_ParseObject()
        {
            // Custom parser implementation
            ICustomParser customParser = new CustomParser();

            // Example usage of ParseObject method
            string valueToParse = "123.45";
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($"Parsed Value: {parsedValue}");

            // Example usage of GetFormat method
            string format = customParser.GetFormat();
            Console.WriteLine($"Format: {format}");
        }
```

### See Also

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


