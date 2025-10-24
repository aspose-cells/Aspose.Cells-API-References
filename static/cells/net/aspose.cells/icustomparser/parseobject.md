##ICustomParser.ParseObject
ICustomParser method. Parses given string to proper value object
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
using Aspose.Cells;
using System;
namespace AsposeCellsExamples
{
public class CustomParser : ICustomParser
{
public object ParseObject(string s)
{
if (double.TryParse(s, out double result))
{
return result;
}
return s;
}
public string GetFormat()
{
return "Numeric or string format";
}
}
public class ICustomParserMethodParseObjectWithStringDemo
{
public static void Run()
{
ICustomParser customParser = new CustomParser();
string valueToParse = "123.45";
object parsedValue = customParser.ParseObject(valueToParse);
Console.WriteLine($"Parsed Value: {parsedValue}");
string format = customParser.GetFormat();
Console.WriteLine($"Format: {format}");
}
}
}
```
### See Also
* interface [ICustomParser](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
