##CustomXmlPart.SchemaData
CustomXmlPart property. Gets or sets the XML content of this Custom XML Schema Data Storage Part
## CustomXmlPart.SchemaData property
Gets or sets the XML content of this Custom XML Schema Data Storage Part.
```csharp
public byte[] SchemaData { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
using System.Text;
public class CustomXmlPartPropertySchemaDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
int index = workbook.CustomXmlParts.Add(null, null);
CustomXmlPart customXmlPart = workbook.CustomXmlParts[index];
Console.WriteLine("Current SchemaData: " + (customXmlPart.SchemaData == null ? "null" : Convert.ToBase64String(customXmlPart.SchemaData)));
string schemaXml = "<?xml version=\"1.0\" encoding=\"UTF-8\"?><xs:schema xmlns:xs=\"http://www.w3.org/2001/XMLSchema\"><xs:element name=\"root\"/></xs:schema>";
byte[] newSchemaData = Encoding.UTF8.GetBytes(schemaXml);
customXmlPart.SchemaData = newSchemaData;
Console.WriteLine("Updated SchemaData: " + Convert.ToBase64String(customXmlPart.SchemaData));
workbook.Save("PropertySchemaDataDemo.xlsx");
}
}
}
```
### See Also
* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
