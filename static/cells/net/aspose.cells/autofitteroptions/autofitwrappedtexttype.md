##AutoFitterOptions.AutoFitWrappedTextType
AutoFitterOptions property. Gets and sets the type of auto fitting wrapped text
## AutoFitterOptions.AutoFitWrappedTextType property
Gets and sets the type of auto fitting wrapped text.
```csharp
public AutoFitWrappedTextType AutoFitWrappedTextType { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyAutoFitWrappedTextTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
cell.Value = "This is a sample text string that demonstrates auto-fitting wrapped text using Paragraph mode";
// Fixed style access using GetStyle/SetStyle pattern
Style style = cell.GetStyle();
style.IsTextWrapped = true;
cell.SetStyle(style);
AutoFitterOptions options = new AutoFitterOptions
{
AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
};
worksheet.AutoFitColumns(options);
workbook.Save("output.html", SaveFormat.Html);
}
}
}
```
### See Also
* enum [AutoFitWrappedTextType](../../autofitwrappedtexttype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
