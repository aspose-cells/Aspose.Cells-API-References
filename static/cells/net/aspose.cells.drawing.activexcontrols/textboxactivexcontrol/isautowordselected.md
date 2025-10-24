##TextBoxActiveXControl.IsAutoWordSelected
TextBoxActiveXControl property. Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word
## TextBoxActiveXControl.IsAutoWordSelected property
Specifies the basic unit used to extend a selection. True specifies that the basic unit is a single character. false specifies that the basic unit is a whole word.
```csharp
public virtual bool IsAutoWordSelected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
namespace AsposeCellsExamples
{
public class TextBoxActiveXControlPropertyIsAutoWordSelectedDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 0, 0, 1, 1, 200, 30);
TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)textBoxShape.ActiveXControl;
Console.WriteLine("Initial IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
if (!textBoxControl.IsAutoWordSelected)
{
textBoxControl.IsAutoWordSelected = true;
}
Console.WriteLine("Final IsAutoWordSelected: " + textBoxControl.IsAutoWordSelected);
}
}
}
```
### See Also
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
