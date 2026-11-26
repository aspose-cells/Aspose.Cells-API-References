---
title: "Enumeración InputMethodEditorMode"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Representa el modo de ejecución predeterminado del Editor de Métodos de Entrada"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Representa el modo de ejecución predeterminado del Editor de Métodos de Entrada.

```csharp
public enum InputMethodEditorMode
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NoControl | `0` | No controla el IME. |
| On | `1` | IME activado. |
| Off | `2` | IME desactivado. Modo inglés. |
| Disable | `3` | IME desactivado. El usuario no puede activar el IME con el teclado. |
| Hiragana | `4` | IME activado con modo hiragana de ancho completo. |
| Katakana | `5` | IME activado con modo katakana de ancho completo. |
| KatakanaHalf | `6` | IME activado con modo katakana de media anchura. |
| AlphaFull | `7` | IME activado con modo alfanumérico de ancho completo. |
| Alpha | `8` | IME activado con modo alfanumérico de media anchura. |
| HangulFull | `9` | IME activado con modo hangul de ancho completo. |
| Hangul | `10` | IME activado con modo hangul de media anchura. |
| HanziFull | `11` | IME activado con modo hanzi de ancho completo. |
| Hanzi | `12` | IME activado con modo hanzi de media anchura. |

### Ejemplos

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
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer el modo IME a hiragana de ancho completo
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Establezca otras propiedades para la demostración
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

            // Guarda el libro de trabajo
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


