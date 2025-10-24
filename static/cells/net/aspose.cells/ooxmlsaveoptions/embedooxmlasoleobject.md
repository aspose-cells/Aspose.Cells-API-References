##OoxmlSaveOptions.EmbedOoxmlAsOleObject
OoxmlSaveOptions property. Indicates whether embedding Ooxml files of OleObject as ole object
## OoxmlSaveOptions.EmbedOoxmlAsOleObject property
Indicates whether embedding Ooxml files of OleObject as ole object.
```csharp
public bool EmbedOoxmlAsOleObject { get; set; }
```
### Remarks
Only for OleObject.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsPropertyEmbedOoxmlAsOleObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample OLE Object Embedding");
// Create OOXML save options and set EmbedOoxmlAsOleObject
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.EmbedOoxmlAsOleObject = true;
// Save the workbook
workbook.Save("output.xlsx", saveOptions);
Console.WriteLine("Workbook saved with OOXML embedded as OLE object.");
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
