##TxtLoadOptions.PreferredParsers
TxtLoadOptions property. Gets and sets preferred value parsers for loading text file
## TxtLoadOptions.PreferredParsers property
Gets and sets preferred value parsers for loading text file.
```csharp
public ICustomParser[] PreferredParsers { get; set; }
```
### Remarks
parsers[0] is the parser will be used for the first column in text template file, parsers[1] is the parser will be used for the second column, ...etc. The last one(parsers[parsers.length-1]) will be used for all other columns start from parsers.length-1. If one item is null, the corresponding column will be parsed by the default parser of Aspose.Cells.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyPreferredParsersDemo
{
private class StringParser : ICustomParser
{
public bool Parse(string value, out object result)
{
result = value; // Always return as string
return true;
}
public object ParseObject(string value)
{
return value; // Always return as string
}
public string GetFormat()
{
return "String"; // Return format description
}
}
public static void Run()
{
// Create CSV load options
TxtLoadOptions options = new TxtLoadOptions(LoadFormat.Csv);
// Set preferred parsers - first try custom string parser, then default parsers
options.PreferredParsers = new ICustomParser[] { new StringParser(), null };
// Sample CSV data with dates
string csvData = "\"2018-10-08\",2018-10-08\n\"2018-10-08\",2018-10-08";
// Load workbook with options
Workbook workbook = new Workbook(new MemoryStream(System.Text.Encoding.UTF8.GetBytes(csvData)), options);
Cells cells = workbook.Worksheets[0].Cells;
// Verify parsing results
Console.WriteLine("A1 Type: " + cells[0, 0].Type); // Should be string
Console.WriteLine("A1 Value: " + cells[0, 0].StringValue); // "2018-10-08"
Console.WriteLine("B1 Type: " + cells[0, 1].Type); // Should be DateTime
Console.WriteLine("B1 Value: " + cells[0, 1].DateTimeValue); // 10/8/2018
}
}
}
```
### See Also
* interface [ICustomParser](../../icustomparser/)
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
