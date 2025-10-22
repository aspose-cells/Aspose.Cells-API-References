##DocxSaveOptions.DocxSaveOptions
DocxSaveOptions constructor. Represents options of saving .docx file
## DocxSaveOptions() {#constructor}
Represents options of saving .docx file.
```csharp
public DocxSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocxSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet and add sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
// Initialize DocxSaveOptions using the constructor
DocxSaveOptions saveOptions = new DocxSaveOptions();
saveOptions.SaveAsEditableShaps = true;
// Save the workbook as DOCX with options
workbook.Save("output.docx", saveOptions);
Console.WriteLine("Document saved successfully with DocxSaveOptions.");
}
}
}
```
### See Also
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## DocxSaveOptions(bool) {#constructor_1}
Represents options of saving .docx file.
```csharp
public DocxSaveOptions(bool saveAsImage)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | Boolean | If True, the workbook will be converted into some pictures of .docx file. If False, the workbook will be converted into some tables of .docx file. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class DocxSaveOptionsMethodCtorWithBooleanDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Save as DOCX with default options
workbook.Save("output_default.docx");
// Save as DOCX with DocxSaveOptions(true) - optimized for MS Word
workbook.Save("output_optimized.docx", new DocxSaveOptions(true));
}
}
}
```
### See Also
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
