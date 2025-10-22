##HtmlTableLoadOptionCollection.TableToListObject
HtmlTableLoadOptionCollection property. Indicates whether generate list objects from imported tables. The default value is false
## HtmlTableLoadOptionCollection.TableToListObject property
Indicates whether generate list objects from imported tables. The default value is false.
```csharp
public bool TableToListObject { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlTableLoadOptionCollectionPropertyTableToListObjectDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Create HtmlLoadOptions
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
// Access the HtmlTableLoadOptionCollection instance
HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;
// Set the TableToListObject property to convert HTML tables to ListObjects
tableLoadOptions.TableToListObject = true;
// Add a table to be converted to ListObject by index
tableLoadOptions.Add(0);
// Load an HTML file into the workbook using the load options
workbook = new Workbook("input.html", loadOptions);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HtmlTableLoadOptionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
