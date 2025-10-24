##Workbook.CustomXmlParts
Workbook property. Represents a Custom XML Data Storage Part custom XML data within a package
## Workbook.CustomXmlParts property
Represents a Custom XML Data Storage Part (custom XML data within a package).
```csharp
public CustomXmlPartCollection CustomXmlParts { get; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyCustomXmlPartsDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Define XML data and schema
string xmlData = "<MyXmlData1 xmlns=\"http://my.namespace.com\"/>";
string xmlSchema = "<?xml version=\"1.0\" encoding=\"UTF-8\" standalone=\"no\"?>" +
"<ds:datastoreItem ds:itemID=\"{1D3CF2F4-9155-40AE-99F6-33298D217F89}\" xmlns:ds=\"http://schemas.openxmlformats.org/officeDocument/2006/customXml\">" +
"<ds:schemaRefs>" +
"<ds:schemaRef ds:uri=\"http://my.namespace.com\"/>" +
"</ds:schemaRefs>" +
"</ds:datastoreItem>";
// Add custom XML part to the workbook
wb.CustomXmlParts.Add(Encoding.UTF8.GetBytes(xmlData), Encoding.UTF8.GetBytes(xmlSchema));
// Save and reload the workbook
string outputPath = "output.xlsx";
wb.Save(outputPath);
Workbook loadedWb = new Workbook(outputPath);
// Display the count of custom XML parts
Console.WriteLine($"Number of custom XML parts: {loadedWb.CustomXmlParts.Count}");
}
}
}
```
### See Also
* class [CustomXmlPartCollection](../../../aspose.cells.markup/customxmlpartcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
