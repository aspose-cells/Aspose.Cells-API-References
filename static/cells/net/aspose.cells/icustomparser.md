##Interface ICustomParser
Aspose.Cells.ICustomParser interface. Allows users to add their custom value parser for parsing string values to other proper cell value object
## ICustomParser interface
Allows users to add their custom value parser for parsing string values to other proper cell value object.
```csharp
public interface ICustomParser
```
## Methods
| Name | Description |
| --- | --- |
| [GetFormat](../../aspose.cells/icustomparser/getformat/)() | Gets the formatting pattern corresponding to the parsed value by last invocation of [`ParseObject`](./parseobject/). |
| [ParseObject](../../aspose.cells/icustomparser/parseobject/)(string) | Parses given string to proper value object. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ICustomParserDemo
{
public static void ICustomParserExample()
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
}
// Custom implementation of ICustomParser
public class CustomParser : ICustomParser
{
private string lastFormat;
public object ParseObject(string value)
{
// Example parsing logic
if (double.TryParse(value, out double result))
{
lastFormat = "0.00"; // Example format
return result;
}
lastFormat = null;
return null;
}
public string GetFormat()
{
return lastFormat;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
