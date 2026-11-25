---
title: "Enum InputMethodEditorMode"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Rappresenta la modalità di runtime predefinita dell'Input Method Editor"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Rappresenta la modalità di runtime predefinita dell'Input Method Editor.

```csharp
public enum InputMethodEditorMode
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| NoControl | `0` | Non controlla l'IME. |
| On | `1` | IME attivo. |
| Off | `2` | IME disattivo. Modalità inglese. |
| Disable | `3` | IME disattivo. L'utente non può attivare l'IME da tastiera. |
| Hiragana | `4` | IME attivo con modalità hiragana a larghezza piena. |
| Katakana | `5` | IME attivo con modalità katakana a larghezza piena. |
| KatakanaHalf | `6` | IME attivo con modalità katakana a larghezza ridotta. |
| AlphaFull | `7` | IME attivo con modalità alfanumerica a larghezza piena. |
| Alpha | `8` | IME attivo con modalità alfanumerica a larghezza ridotta. |
| HangulFull | `9` | IME attivo con modalità hangul a larghezza piena. |
| Hangul | `10` | IME attivo con modalità hangul a larghezza ridotta. |
| HanziFull | `11` | IME attivo con modalità hanzi a larghezza piena. |
| Hanzi | `12` | IME attivo con modalità hanzi a larghezza ridotta. |

### Esempi

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
            // Inizializza una nuova cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un controllo ActiveX TextBox al foglio di lavoro
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Imposta la modalità IME su Hiragana a larghezza piena
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Imposta altre proprietà per la dimostrazione
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

            // Salva la cartella di lavoro
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


