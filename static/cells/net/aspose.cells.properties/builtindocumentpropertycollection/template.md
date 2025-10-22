##BuiltInDocumentPropertyCollection.Template
BuiltInDocumentPropertyCollection property. Gets or sets the informational name of the document template
## BuiltInDocumentPropertyCollection.Template property
Gets or sets the informational name of the document template.
```csharp
public string Template { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the built-in document properties
BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;
// Set the Template property
builtInProperties.Template = "Standard Template";
// Set other basic properties for demonstration
builtInProperties.Author = "John Doe";
builtInProperties.Title = "Template Property Demo";
// Save the workbook
workbook.Save("TemplatePropertyDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
