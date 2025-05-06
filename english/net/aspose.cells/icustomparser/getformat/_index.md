---
title: ICustomParser.GetFormat
second_title: Aspose.Cells for .NET API Reference
description: ICustomParser method. Gets the formatting pattern corresponding to the parsed value by last invocation of ParseObject
type: docs
url: /net/aspose.cells/icustomparser/getformat/
---
## ICustomParser.GetFormat method

Gets the formatting pattern corresponding to the parsed value by last invocation of [`ParseObject`](../parseobject/).

```csharp
public string GetFormat()
```

### Remarks

The returned formatting pattern may be used to format corresponding cell(set to Style.Custom for the cell).

### Examples

```csharp
// Called: string format = customParser.GetFormat();
public static void Method_GetFormat()
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


