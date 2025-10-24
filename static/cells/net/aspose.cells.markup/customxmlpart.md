##Class CustomXmlPart
Aspose.Cells.Markup.CustomXmlPart class. Represents a Custom XML Data Storage Part custom XML data within a package
## CustomXmlPart class
Represents a Custom XML Data Storage Part (custom XML data within a package).
```csharp
public class CustomXmlPart
```
## Properties
| Name | Description |
| --- | --- |
| [Data](../../aspose.cells.markup/customxmlpart/data/) { get; set; } | Gets or sets the XML content of this Custom XML Data Storage Part. |
| [ID](../../aspose.cells.markup/customxmlpart/id/) { get; set; } | Gets and sets the id of the custom xml part. |
| [SchemaData](../../aspose.cells.markup/customxmlpart/schemadata/) { get; set; } | Gets or sets the XML content of this Custom XML Schema Data Storage Part. |
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class MarkupClassCustomXmlPartDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
CustomXmlPartCollection xmlParts = workbook.CustomXmlParts;
string xmlData = "<root><item>Sample Data</item></root>";
byte[] dataBytes = Encoding.UTF8.GetBytes(xmlData);
string originalId = Guid.NewGuid().ToString();
int index = xmlParts.Add(dataBytes, null);
CustomXmlPart newPart = xmlParts[index];
newPart.ID = originalId;
Console.WriteLine("Original ID: " + originalId);
Console.WriteLine("Stored ID: " + newPart.ID);
string newId = Guid.NewGuid().ToString();
newPart.ID = newId;
Console.WriteLine("Updated ID: " + newId);
workbook.Save("output.xlsx");
Workbook loadedWorkbook = new Workbook("output.xlsx");
CustomXmlPart retrievedPart = loadedWorkbook.CustomXmlParts.SelectByID(newId);
Console.WriteLine("Retrieved ID: " + (retrievedPart != null ? retrievedPart.ID : "Not found"));
}
}
}
```
### See Also
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
