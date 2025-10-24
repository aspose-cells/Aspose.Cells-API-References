##AutoFitterOptions.DefaultEditLanguage
AutoFitterOptions property. Gets or sets default edit language
## AutoFitterOptions.DefaultEditLanguage property
Gets or sets default edit language.
```csharp
public DefaultEditLanguage DefaultEditLanguage { get; set; }
```
### Remarks
It may display/render different layouts for text paragraph when different edit languages is set. Default is Auto.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyDefaultEditLanguageDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample CJK text in a cell
worksheet.Cells["A1"].PutValue("日本語のテキスト");
AutoFitterOptions options = new AutoFitterOptions();
options.DefaultEditLanguage = DefaultEditLanguage.CJK;
// Auto-fit row with CJK language settings
worksheet.AutoFitRows(options);
Console.WriteLine("Auto-fit completed with DefaultEditLanguage: " + options.DefaultEditLanguage);
workbook.Save("DefaultEditLanguageDemo.xlsx");
}
}
}
```
### See Also
* enum [DefaultEditLanguage](../../defaulteditlanguage/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
