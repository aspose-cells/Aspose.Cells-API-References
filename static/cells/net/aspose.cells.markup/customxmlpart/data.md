##CustomXmlPart.Data
CustomXmlPart property. Gets or sets the XML content of this Custom XML Data Storage Part
## CustomXmlPart.Data property
Gets or sets the XML content of this Custom XML Data Storage Part.
```csharp
public byte[] Data { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Markup;
using System;
using System.Text;
public class CustomXmlPartPropertyDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
byte[] initialData = Encoding.UTF8.GetBytes("<root><data>Initial Value</data></root>");
int xmlPartIndex = workbook.CustomXmlParts.Add(initialData, null);
CustomXmlPart xmlPart = workbook.CustomXmlParts[xmlPartIndex];
Console.WriteLine("Current Data value: " + Encoding.UTF8.GetString(xmlPart.Data));
xmlPart.Data = Encoding.UTF8.GetBytes("<root><data>Modified Value</data></root>");
workbook.CustomXmlParts.Add(xmlPart.Data, null);
workbook.Save("CustomXmlPartDataDemo.xlsx");
}
}
}
```
### See Also
* class [CustomXmlPart](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)
