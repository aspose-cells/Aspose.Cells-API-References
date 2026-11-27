---
title: "Enum InputMethodEditorMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Representerar standardkörningsläget för Input Method Editor"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Representerar standardkörningsläget för Input Method Editor.

```csharp
public enum InputMethodEditorMode
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| NoControl | `0` | Styr inte IME. |
| On | `1` | IME på. |
| Off | `2` | IME av. Engelsk läge. |
| Disable | `3` | IME av. Användaren kan inte slå på IME via tangentbordet. |
| Hiragana | `4` | IME på med fullbredd hiragana-läge. |
| Katakana | `5` | IME på med fullbredd katakana-läge. |
| KatakanaHalf | `6` | IME på med halvbred katakana-läge. |
| AlphaFull | `7` | IME på med fullbredd alfanumeriskt läge. |
| Alpha | `8` | IME på med halvbred alfanumeriskt läge. |
| HangulFull | `9` | IME på med fullbredd hangul-läge. |
| Hangul | `10` | IME på med halvbred hangul-läge. |
| HanziFull | `11` | IME på med fullbredd hanzi-läge. |
| Hanzi | `12` | IME på med halvbred hanzi-läge. |

### Exempel

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
            // Initiera en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en TextBox ActiveX-kontroll till kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Ställ in IME-läget till fullbredd Hiragana
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Ställ in andra egenskaper för demonstration
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

            // Spara arbetsboken
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


