##DocumentProperty.ToDouble
DocumentProperty method. Returns the property value as double
## DocumentProperty.ToDouble method
Returns the property value as double.
```csharp
public double ToDouble()
```
### Remarks
Throws an exception if the property type is not PropertyType.Float.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;
namespace AsposeCellsExamples
{
public class DocumentPropertyMethodToDoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Get custom document properties collection
CustomDocumentPropertyCollection customProperties = workbook.Worksheets.CustomDocumentProperties;
// Add a numeric property
customProperties.Add("Rating", 4.75);
// Get the property and convert to double
DocumentProperty ratingProperty = customProperties["Rating"];
double ratingValue = ratingProperty.ToDouble();
// Output the result
Console.WriteLine($"Rating: {ratingValue}");
// Save the workbook
workbook.Save("DocumentPropertyToDoubleExample.xlsx");
}
}
}
```
### See Also
* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)
