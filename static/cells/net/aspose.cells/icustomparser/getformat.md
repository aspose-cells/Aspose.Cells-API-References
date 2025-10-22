##ICustomParser.GetFormat
ICustomParser method. Gets the formatting pattern corresponding to the parsed value by last invocation of ParseObject
## ICustomParser.GetFormat method
Gets the formatting pattern corresponding to the parsed value by last invocation of [`ParseObject`](../parseobject/).
```csharp
public string GetFormat()
```
### Remarks
The returned formatting pattern may be used to format corresponding cell(set to Style.Custom for the cell).
### Examples
```csharp
using Aspose.Cells;
using System;
namespace AsposeCellsExamples
{
public class CustomParser2 : ICustomParser
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
return "Standard numeric format";
}
}
public class ICustomParser1MethodGetFormatDemo
{
public static void Run()
{
ICustomParser customParser = new CustomParser2();
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
