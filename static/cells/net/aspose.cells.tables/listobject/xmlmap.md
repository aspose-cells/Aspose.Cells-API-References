##ListObject.XmlMap
ListObject property. Gets an XmlMap used for this list
## ListObject.XmlMap property
Gets an `XmlMap` used for this list.
```csharp
public XmlMap XmlMap { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectPropertyXmlMapDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["B3"].PutValue(1.5);
// Create a list object (table)
int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject listObject = worksheet.ListObjects[index];
listObject.DisplayName = "ProductTable";
// Add XML map to the workbook
string xmlSchema = @"<xs:schema xmlns:xs='http://www.w3.org/2001/XMLSchema'>
// Fixed: Use correct overload for XmlMaps.Add
int mapIndex = workbook.Worksheets.XmlMaps.Add(xmlSchema);
XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
xmlMap.Name = "Products";
// Fixed: Cannot assign to XmlMap as it's read-only, so we need to use the XML map when creating the table
// or find another way to associate the table with the XML map
// For demo purposes, we'll just show the existing XmlMap info if available
if (listObject.XmlMap != null)
{
Console.WriteLine("XML Map Name: " + listObject.XmlMap.Name);
Console.WriteLine("Root Element: " + listObject.XmlMap.RootElementName);
}
// Save the workbook
workbook.Save("ListObjectWithXmlMap.xlsx");
}
}
}
```
### See Also
* class [XmlMap](../../../aspose.cells/xmlmap/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
