##DocxSaveOptions.SaveAsEditableShaps
DocxSaveOptions property. Save all drawing objecgts as editable shapes in word file.So you can edit them in Word
## DocxSaveOptions.SaveAsEditableShaps property
Save all drawing objecgts as editable shapes in word file.So you can edit them in Word.
```csharp
[Obsolete("Use SaveFormat.SaveAsEditableShapes instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool SaveAsEditableShaps { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use [`SaveAsEditableShapes`](../saveaseditableshapes/) property. This property will be removed 6 months later since May 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocxSaveOptionsPropertySaveAsEditableShapsDemo
{
public static void Run()
{
// Create a workbook object and open the template Excel file
Workbook workbook = new Workbook("example.xlsx");
// Initialize DocxSaveOptions
DocxSaveOptions saveOptions = new DocxSaveOptions();
// Set SaveAsEditableShaps property to true
saveOptions.SaveAsEditableShaps = true;
// Save the workbook as DOCX with the specified options
workbook.Save("example.docx", saveOptions);
}
}
}
```
### See Also
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
