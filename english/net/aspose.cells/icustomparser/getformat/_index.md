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


