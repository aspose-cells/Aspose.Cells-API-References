##HtmlSaveOptions.PresentationPreference
HtmlSaveOptions property. Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentationplease set the value to true
## HtmlSaveOptions.PresentationPreference property
Indicating if html or mht file is presentation preference. The default value is false. if you want to get more beautiful presentation,please set the value to true.
```csharp
public bool PresentationPreference { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyPresentationPreferenceDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Presentation Preference Test");
worksheet.Cells["B1"].PutValue(123.45);
worksheet.Cells["A2"].PutValue(DateTime.Now);
// Set HTML save options with PresentationPreference
HtmlSaveOptions options = new HtmlSaveOptions();
options.PresentationPreference = true;
options.IsFullPathLink = false;
// Save to memory stream for demonstration
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, options);
Console.WriteLine("Workbook saved with PresentationPreference=true");
}
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
