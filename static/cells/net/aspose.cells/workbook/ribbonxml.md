##Workbook.RibbonXml
Workbook property. Gets and sets the XML file that defines the Ribbon UI
## Workbook.RibbonXml property
Gets and sets the XML file that defines the Ribbon UI.
```csharp
public string RibbonXml { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookPropertyRibbonXmlDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Sample ribbon XML to customize the ribbon
string ribbonXml =
"<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
"  <ribbon>" +
"    <tabs>" +
"      <tab id=\"customTab\" label=\"My Tab\">" +
"        <group id=\"customGroup\" label=\"My Group\">" +
"          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
"        </group>" +
"      </tab>" +
"    </tabs>" +
"  </ribbon>" +
"</customUI>";
// Set the RibbonXml property
workbook.RibbonXml = ribbonXml;
// Save the workbook
workbook.Save("output.xlsm");
// Verify the RibbonXml property
Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
