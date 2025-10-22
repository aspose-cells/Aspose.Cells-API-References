##Worksheet.Replace
Worksheet method. Replaces all cells text with a new string
## Worksheet.Replace method
Replaces all cells' text with a new string.
```csharp
public int Replace(string oldString, string newString)
```
| Parameter | Type | Description |
| --- | --- | --- |
| oldString | String | Old string value. |
| newString | String | New string value. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodReplaceWithStringStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Hello World");
worksheet.Cells["A2"].PutValue("Hello Aspose");
worksheet.Cells["A3"].PutValue("Hello Cells");
// Add textbox with sample text
worksheet.TextBoxes.Add(5, 0, 100, 50);
worksheet.TextBoxes[0].Text = "Hello TextBox";
// Set header and footer
worksheet.PageSetup.SetHeader(0, "Hello Header");
worksheet.PageSetup.SetFooter(0, "Hello Footer");
// Replace "Hello" with "Hi" in all content
string findText = "Hello";
string replaceText = "Hi";
worksheet.Replace(findText, replaceText);
// Replace in headers/footers
for (int i = 0; i < 3; i++)
{
if (worksheet.PageSetup.GetHeader(i) != null)
worksheet.PageSetup.SetHeader(i, worksheet.PageSetup.GetHeader(i).Replace(findText, replaceText));
if (worksheet.PageSetup.GetFooter(i) != null)
worksheet.PageSetup.SetFooter(i, worksheet.PageSetup.GetFooter(i).Replace(findText, replaceText));
}
// Replace in textboxes
foreach (Aspose.Cells.Drawing.TextBox textBox in worksheet.TextBoxes)
{
if (textBox.Text != null)
{
textBox.Text = textBox.Text.Replace(findText, replaceText);
}
}
// Save the workbook
workbook.Save("ReplaceDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
