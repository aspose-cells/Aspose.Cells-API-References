##BuiltInDocumentPropertyCollection.Manager
BuiltInDocumentPropertyCollection property. Gets or sets the manager property
## BuiltInDocumentPropertyCollection.Manager property
Gets or sets the manager property.
```csharp
public string Manager { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyManagerDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set core document properties including Manager
builtInProperties.Author = "John Doe";
builtInProperties.Title = "Sample Workbook";
builtInProperties.Manager = "Jane Smith"; // Demonstrating Manager property usage
builtInProperties.Company = "Aspose";
// Save the workbook
workbook.Save("DocumentPropertiesDemo.xlsx");
Console.WriteLine("Workbook created with Manager property set to: " + builtInProperties.Manager);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
