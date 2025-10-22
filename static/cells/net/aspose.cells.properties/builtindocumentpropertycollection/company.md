##BuiltInDocumentPropertyCollection.Company
BuiltInDocumentPropertyCollection property. Gets or sets the company property
## BuiltInDocumentPropertyCollection.Company property
Gets or sets the company property.
```csharp
public string Company { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyCompanyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Set built-in document properties including Company
workbook.BuiltInDocumentProperties.Title = "Annual Report";
workbook.BuiltInDocumentProperties.Company = "Contoso Ltd";
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx");
// Display the set properties
Console.WriteLine("Title: " + workbook.BuiltInDocumentProperties.Title);
Console.WriteLine("Company: " + workbook.BuiltInDocumentProperties.Company);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
