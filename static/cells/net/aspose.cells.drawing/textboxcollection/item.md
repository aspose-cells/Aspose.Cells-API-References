##TextBoxCollection.Item
TextBoxCollection property. Gets the TextBox element at the specified index
## TextBoxCollection indexer (1 of 2)
Gets the [`TextBox`](../../textbox/) element at the specified index.
```csharp
public TextBox this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxCollectionPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some textboxes to the worksheet
int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
textBox1.Text = "TextBox 1";
int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
textBox2.Text = "TextBox 2";
// Access textboxes using Item property
TextBoxCollection textBoxCollection = worksheet.TextBoxes;
int index = textBoxCollection.Count - 1;
TextBox lastTextBox = textBoxCollection[index];
// Output the text of the last textbox
Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
}
}
}
```
### See Also
* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
## TextBoxCollection indexer (2 of 2)
Gets the [`TextBox`](../../textbox/) element by the name.
```csharp
public TextBox this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The name of the text box. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class TextBoxCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add textboxes to the worksheet and get their indices
int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
textBox1.Name = "textbox 1";
textBox1.Text = "First TextBox";
int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
textBox2.Name = "textbox 2";
textBox2.Text = "Second TextBox";
// Access textbox using Item property by name
string txtboxName = "textbox 1";
TextBox txb2 = worksheet.TextBoxes[txtboxName];
if (txb2 != null)
{
Console.WriteLine("Found TextBox: " + txb2.Name);
Console.WriteLine("TextBox Text: " + txb2.Text);
}
}
}
}
```
### See Also
* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
