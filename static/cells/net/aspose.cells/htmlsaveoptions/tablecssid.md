##HtmlSaveOptions.TableCssId
HtmlSaveOptions property. Gets and sets the prefix of the type css name such as trcoltd and so on they are contained in the table element which has the specific TableCssId attribute. The default value is
## HtmlSaveOptions.TableCssId property
Gets and sets the prefix of the type css name such as tr,col,td and so on, they are contained in the table element which has the specific TableCssId attribute. The default value is "".
```csharp
public string TableCssId { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyTableCssIdDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Configure HTML save options with TableCssId
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
saveOptions.TableCssId = "custom-table-style";
// Save the workbook with HTML options
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML file saved with TableCssId: " + saveOptions.TableCssId);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
