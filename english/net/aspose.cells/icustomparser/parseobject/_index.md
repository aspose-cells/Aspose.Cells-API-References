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
public static void Method_String_()
        {
            // Custom parser implementation
            ICustomParser customParser = new CustomParser();

            // Example usage of ParseObject method
            string valueToParse = &quot;123.45&quot;;
            object parsedValue = customParser.ParseObject(valueToParse);
            Console.WriteLine($&quot;Parsed Value: {parsedValue}&quot;);

            // Example usage of GetFormat method
            string format = customParser.GetFormat();
            Console.WriteLine($&quot;Format: {format}&quot;);
        }
```

### See Also

* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


