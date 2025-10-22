##Enum InputMethodEditorMode
Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Represents the default runtime mode of the Input Method Editor
## InputMethodEditorMode enumeration
Represents the default run-time mode of the Input Method Editor.
```csharp
public enum InputMethodEditorMode
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| NoControl | `0` | Does not control IME. |
| On | `1` | IME on. |
| Off | `2` | IME off. English mode. |
| Disable | `3` | IME off.User can't turn on IME by keyboard. |
| Hiragana | `4` | IME on with Full-width hiragana mode. |
| Katakana | `5` | IME on with Full-width katakana mode. |
| KatakanaHalf | `6` | IME on with Half-width katakana mode. |
| AlphaFull | `7` | IME on with Full-width Alphanumeric mode. |
| Alpha | `8` | IME on with Half-width Alphanumeric mode. |
| HangulFull | `9` | IME on with Full-width hangul mode. |
| Hangul | `10` | IME on with Half-width hangul mode. |
| HanziFull | `11` | IME on with Full-width hanzi mode. |
| Hanzi | `12` | IME on with Half-width hanzi mode. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class InputMethodEditorModeDemo
{
public static void InputMethodEditorModeExample()
{
// Initialize a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a TextBox ActiveX control to the worksheet
Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;
// Set the IME mode to Full-width Hiragana
textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;
// Set other properties for demonstration
textBoxControl.Text = "This is a test.";
textBoxControl.IsEnabled = true;
textBoxControl.IsLocked = false;
textBoxControl.IsTransparent = false;
textBoxControl.IsAutoSize = true;
textBoxControl.Width = 200;
textBoxControl.Height = 50;
textBoxControl.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
textBoxControl.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.White);
textBoxControl.IsVisible = true;
textBoxControl.Shadow = false;
// Save the workbook
workbook.Save("InputMethodEditorModeExample.xlsx");
workbook.Save("InputMethodEditorModeExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)
