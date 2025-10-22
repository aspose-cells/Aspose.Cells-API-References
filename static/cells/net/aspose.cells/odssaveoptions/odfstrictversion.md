##OdsSaveOptions.OdfStrictVersion
OdsSaveOptions property. Gets and sets the ODF version
## OdsSaveOptions.OdfStrictVersion property
Gets and sets the ODF version.
```csharp
public OpenDocumentFormatVersionType OdfStrictVersion { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Ods;
namespace AsposeCellsExamples
{
public class OdsSaveOptionsPropertyOdfStrictVersionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("ODF Version Demo");
// Create ODS save options
OdsSaveOptions saveOptions = new OdsSaveOptions();
// Set ODF version to 1.2
saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
// Save with specified ODF version
workbook.Save("OdfVersion12.ods", saveOptions);
// Change to ODF version 1.3
saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf13;
workbook.Save("OdfVersion13.ods", saveOptions);
}
}
}
```
### See Also
* enum [OpenDocumentFormatVersionType](../../../aspose.cells.ods/opendocumentformatversiontype/)
* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
