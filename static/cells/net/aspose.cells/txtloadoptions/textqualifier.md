##TxtLoadOptions.TextQualifier
TxtLoadOptions property. Specifies the text qualifier for cell values. Default qualifier is
## TxtLoadOptions.TextQualifier property
Specifies the text qualifier for cell values. Default qualifier is '"'.
```csharp
public char TextQualifier { get; set; }
```
### Remarks
When setting this property, [`HasTextQualifier`](../hastextqualifier/) will become true automatically.
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyTextQualifierDemo
{
public static void Run()
{
// Create an instance of TxtLoadOptions for CSV
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
Separator = ',',
HasTextQualifier = true,
TextQualifier = '\"'
};
// Create sample CSV data with text qualifiers
string csvData = "Name,Age,City\n\"John Doe\",30,\"New York\"\n\"Jane Smith\",25,\"San Francisco\"";
// Save sample data to a temporary file
string tempFile = "temp.csv";
System.IO.File.WriteAllText(tempFile, csvData);
// Load the CSV file with the specified options
Workbook workbook = new Workbook(tempFile, loadOptions);
// Save the workbook to an Excel file
workbook.Save("TextQualifierDemo.xlsx");
// Clean up temporary file
System.IO.File.Delete(tempFile);
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
