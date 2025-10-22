##HtmlSaveOptions.ExportObjectListener
HtmlSaveOptions property. Gets or sets the ExportObjectListener for exporting objects
## HtmlSaveOptions.ExportObjectListener property
Gets or sets the ExportObjectListener for exporting objects.
```csharp
[Obsolete("Use HtmlSaveOptions.IStreamProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IExportObjectListener ExportObjectListener { get; set; }
```
### Remarks
NOTE: This property is now obsolete. Instead, please use HtmlSaveOptions.IStreamProvider property. This property will be removed 12 months later since August 2015. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportObjectListenerDemo
{
public static void Run()
{
// Create a custom export object listener
var listener = new CustomExportObjectListener();
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Export Object Listener");
// Create HTML save options with the listener
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
ExportObjectListener = listener
};
// Save to HTML file
workbook.Save("output.html", saveOptions);
}
}
// Custom implementation of IExportObjectListener
public class CustomExportObjectListener : IExportObjectListener
{
public object ExportObject(ExportObjectEvent e)
{
// Example: Process the exported object
Console.WriteLine($"Exporting object: {e.GetType()}");
// Return the original object (could modify it if needed)
return e;
}
}
}
```
### See Also
* interface [IExportObjectListener](../../iexportobjectlistener/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
