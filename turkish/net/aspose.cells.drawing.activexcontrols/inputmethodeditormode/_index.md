---
title: "Enum InputMethodEditorMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Giriş Yöntemi Düzenleyicisinin varsayılan çalışma zaman modunu temsil eder"
type: docs
url: /tr/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Input Method Editor'in varsayılan çalışma zamanı modunu temsil eder.

```csharp
public enum InputMethodEditorMode
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| NoControl | `0` | IME'yi kontrol etmez. |
| On | `1` | IME açık. |
| Off | `2` | IME kapalı. İngilizce modu. |
| Disable | `3` | IME kapalı.Kullanıcı klavye ile IME'yi açamaz. |
| Hiragana | `4` | IME açık, Tam genişlik hiragana modu ile. |
| Katakana | `5` | IME açık, Tam genişlik katakana modu ile. |
| KatakanaHalf | `6` | IME açık, Yarım genişlik katakana modu ile. |
| AlphaFull | `7` | IME açık, Tam genişlik Alfanümerik modu ile. |
| Alpha | `8` | IME açık, Yarım genişlik Alfanümerik modu ile. |
| HangulFull | `9` | IME açık, Tam genişlik Hangul modu ile. |
| Hangul | `10` | IME açık, Yarım genişlik Hangul modu ile. |
| HanziFull | `11` | IME açık, Tam genişlik Hanzi modu ile. |
| Hanzi | `12` | IME açık, Yarım genişlik Hanzi modu ile. |

### Örnekler

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
            // Yeni bir çalışma kitabı başlat
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir TextBox ActiveX denetimi ekle
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // IME modunu Tam genişlik Hiragana olarak ayarla
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Demonstrasyon için diğer özellikleri ayarlayın
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

            // Çalışma kitabını kaydedin
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


