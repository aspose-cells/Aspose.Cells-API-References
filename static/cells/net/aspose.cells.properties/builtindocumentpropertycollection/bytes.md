##BuiltInDocumentPropertyCollection.Bytes
BuiltInDocumentPropertyCollection property. Represents an estimate of the number of bytes in the document
## BuiltInDocumentPropertyCollection.Bytes property
Represents an estimate of the number of bytes in the document.
```csharp
[Obsolete("This property is written for Word and PowerPoint. Excel will omit this property")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Bytes { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Properties;
using System;
public class BuiltInDocumentPropertyCollectionPropertyBytesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access built-in document properties
BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;
// Display current Bytes value (estimate of document size)
Console.WriteLine("Current Bytes value: " + properties.Bytes);
// Add some content to affect the size
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample data to increase document size");
for (int i = 2; i <= 100; i++)
{
worksheet.Cells["A" + i].PutValue("Line " + i);
}
// Update the Bytes property manually (though normally this would be auto-calculated)
properties.Bytes = 5000;
Console.WriteLine("Updated Bytes value: " + properties.Bytes);
// Save the workbook to see the property in the saved file
workbook.Save("PropertyBytesDemo.xlsx");
}
}
}
```
### See Also
* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
