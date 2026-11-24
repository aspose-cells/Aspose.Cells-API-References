---
title: "Enum InputMethodEditorMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Stellt den Standardlaufzeitmodus des Eingabemethoden‑Editors dar"
type: docs
url: /de/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Stellt den Standardlaufzeitmodus des Eingabemethoden-Editors dar.

```csharp
public enum InputMethodEditorMode
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| NoControl | `0` | Steuert IME nicht. |
| On | `1` | IME an. |
| Off | `2` | IME aus. Englischer Modus. |
| Disable | `3` | IME aus. Der Benutzer kann IME nicht über die Tastatur aktivieren. |
| Hiragana | `4` | IME an im Vollbreiten‑Hiragana‑Modus. |
| Katakana | `5` | IME an im Vollbreiten‑Katakana‑Modus. |
| KatakanaHalf | `6` | IME an im Halbbreiten‑Katakana‑Modus. |
| AlphaFull | `7` | IME an im Vollbreiten‑Alphanumerischen Modus. |
| Alpha | `8` | IME an mit halbbreitem alphanumerischem Modus. |
| HangulFull | `9` | IME an mit vollbreitem Hangul-Modus. |
| Hangul | `10` | IME an mit halbbreitem Hangul-Modus. |
| HanziFull | `11` | IME an mit vollbreitem Hanzi-Modus. |
| Hanzi | `12` | IME an mit halbbreitem Hanzi-Modus. |

### Beispiele

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
            // Initialisieren Sie ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein TextBox ActiveX-Steuerelement zum Arbeitsblatt hinzu
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Setzen Sie den IME-Modus auf vollbreites Hiragana
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Legen Sie weitere Eigenschaften zur Demonstration fest
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

            // Speichere die Arbeitsmappe
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


