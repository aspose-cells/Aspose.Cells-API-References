##DocumentPropertyCollection.Remove
DocumentPropertyCollection method. Removes a property with the specified name from the collection
## DocumentPropertyCollection.Remove method
Removes a property with the specified name from the collection.
```csharp
public void Remove(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The case-insensitive name of the property. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocumentPropertyCollectionMethodRemoveWithStringDemo
{
public static void Run()
{
string inputPath = "example.xlsx";
string outputPath = "output.xlsm";
using (FileStream stream = new FileStream(inputPath, FileMode.Open))
{
Workbook workbook = new Workbook(stream);
if (workbook.Worksheets.CustomDocumentProperties.Contains("_PID_HLINKS"))
{
workbook.Worksheets.CustomDocumentProperties.Remove("_PID_HLINKS");
}
workbook.Save(outputPath, SaveFormat.Xlsm);
}
}
}
}
```
### See Also
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
