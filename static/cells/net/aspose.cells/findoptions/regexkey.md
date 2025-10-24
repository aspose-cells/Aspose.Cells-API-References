##FindOptions.RegexKey
FindOptions property. Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel
## FindOptions.RegexKey property
Indicates whether the searched key is regex. If true the searched key will be taken as regex and parsed. Otherwise the key will be parsed according to the rules in ms excel.
```csharp
public bool RegexKey { get; set; }
```
### Remarks
Even though the search key has been specified as regex, it may be refactored according to specified [`LookAtType`](../lookattype/). For example, when the type is Contains(this is the default value for this options), wildcards will be added at the beginning and end of the search key automatically to ensure the match will be checked as "contains". In this case, the regular expressions will become more complex and the performance will also decrease. So, for performance consideration, if user has specified the exact rule for the regex, then there is no need to use [`LookAtType`](../lookattype/) as additional constraint and user may set it as EntireContent to get better performance.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyRegexKeyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set test data with pattern matching strings
worksheet.Cells["A1"].PutValue("[hello]");
worksheet.Cells["A2"].PutValue("Regular text");
worksheet.Cells["A3"].PutValue("[another_example]");
// Create find options with regex enabled
FindOptions options = new FindOptions();
options.RegexKey = true;
options.LookInType = LookInType.Values;
options.LookAtType = LookAtType.Contains;
// Search for cells matching the regex pattern
string regEx = "\\[[a-zA-Z0-9_]+\\]";
Cell foundCell = worksheet.Cells.Find(regEx, null, options);
// Output the result
if (foundCell != null)
{
Console.WriteLine("Found cell: " + foundCell.Name + " with value: " + foundCell.StringValue);
}
else
{
Console.WriteLine("No matching cells found");
}
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
