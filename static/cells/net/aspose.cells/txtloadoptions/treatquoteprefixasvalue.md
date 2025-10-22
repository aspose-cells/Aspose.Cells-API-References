##TxtLoadOptions.TreatQuotePrefixAsValue
TxtLoadOptions property. Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false the leading single quote will be removed from corresponding cells value and QuotePrefix will be set as true for the cell
## TxtLoadOptions.TreatQuotePrefixAsValue property
Indicates whether the leading single quote sign should be taken as part of the value of one cell. Default is true. If it is false, the leading single quote will be removed from corresponding cell's value and [`QuotePrefix`](../../style/quoteprefix/) will be set as true for the cell.
```csharp
public bool TreatQuotePrefixAsValue { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyTreatQuotePrefixAsValueDemo
{
public static void Run()
{
// Create sample CSV data with quote prefixes
string csvData = "ID,Name,Value\n1,\"'Apple\",100\n2,\"'Orange\",200";
string filePath = "test.csv";
// Save the CSV data to a file
File.WriteAllText(filePath, csvData);
// Scenario 1: TreatQuotePrefixAsValue = false (default)
var loadOptions1 = new TxtLoadOptions();
loadOptions1.TreatQuotePrefixAsValue = false;
var workbook1 = new Workbook(filePath, loadOptions1);
var worksheet1 = workbook1.Worksheets[0];
Console.WriteLine("TreatQuotePrefixAsValue = false:");
Console.WriteLine("Cell B2 value: " + worksheet1.Cells["B2"].Value); // Will show 'Apple (quote treated as formatting)
// Scenario 2: TreatQuotePrefixAsValue = true
var loadOptions2 = new TxtLoadOptions();
loadOptions2.TreatQuotePrefixAsValue = true;
var workbook2 = new Workbook(filePath, loadOptions2);
var worksheet2 = workbook2.Worksheets[0];
Console.WriteLine("\nTreatQuotePrefixAsValue = true:");
Console.WriteLine("Cell B2 value: " + worksheet2.Cells["B2"].Value); // Will show 'Apple (quote treated as value)
// Clean up
File.Delete(filePath);
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
