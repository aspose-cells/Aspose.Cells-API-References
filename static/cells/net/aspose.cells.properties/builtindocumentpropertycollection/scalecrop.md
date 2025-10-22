##BuiltInDocumentPropertyCollection.ScaleCrop
BuiltInDocumentPropertyCollection property. Indicates the display mode of the document thumbnail
## BuiltInDocumentPropertyCollection.ScaleCrop property
Indicates the display mode of the document thumbnail.
```csharp
public bool ScaleCrop { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class BuiltInDocumentPropertyCollectionPropertyScaleCropDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Set ScaleCrop property
properties.ScaleCrop = true;
// Display the ScaleCrop property value
Console.WriteLine("ScaleCrop property value: " + properties.ScaleCrop);
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
