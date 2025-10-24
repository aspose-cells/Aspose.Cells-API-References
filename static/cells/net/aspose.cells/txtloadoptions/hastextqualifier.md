##TxtLoadOptions.HasTextQualifier
TxtLoadOptions property. Whether there is text qualifier for cell value. Default is true
## TxtLoadOptions.HasTextQualifier property
Whether there is text qualifier for cell value. Default is true.
```csharp
public bool HasTextQualifier { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyHasTextQualifierDemo
{
public static void Run()
{
// Create CSV content with text qualifiers
string csvContent = "\"Name\",\"Age\",\"City\"\n\"John\",30,\"New York\"\n\"Alice\",25,\"London\"";
// Save CSV content to a temporary file
string tempFile = "temp.csv";
System.IO.File.WriteAllText(tempFile, csvContent, Encoding.UTF8);
// Create TxtLoadOptions with HasTextQualifier set to true
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
Separator = ',',
HasTextQualifier = true,
TextQualifier = '\"'
};
// Load the CSV file with text qualifiers
Workbook workbook = new Workbook(tempFile, loadOptions);
// Save the workbook to demonstrate successful loading
workbook.Save("Output.xlsx");
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
