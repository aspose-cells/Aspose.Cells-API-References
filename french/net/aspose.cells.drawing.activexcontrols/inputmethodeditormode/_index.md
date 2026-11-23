---
title: "Énum InputMethodEditorMode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode enum. Représente le mode d'exécution par défaut de l'éditeur de méthodes d'entrée"
type: docs
url: /fr/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

Représente le mode d'exécution par défaut de l'éditeur de méthodes d'entrée.

```csharp
public enum InputMethodEditorMode
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| NoControl | `0` | Ne contrôle pas l'IME. |
| On | `1` | IME activé. |
| Off | `2` | IME désactivé. Mode anglais. |
| Disable | `3` | IME désactivé. L'utilisateur ne peut pas activer l'IME via le clavier. |
| Hiragana | `4` | IME activé avec le mode hiragana pleine largeur. |
| Katakana | `5` | IME activé avec le mode katakana pleine largeur. |
| KatakanaHalf | `6` | IME activé avec le mode katakana demi-largeur. |
| AlphaFull | `7` | IME activé avec le mode alphanumérique pleine largeur. |
| Alpha | `8` | IME activé avec le mode alphanumérique demi-largeur. |
| HangulFull | `9` | IME activé avec le mode hangul pleine largeur. |
| Hangul | `10` | IME activé avec le mode hangul demi-largeur. |
| HanziFull | `11` | IME activé avec le mode hanzi pleine largeur. |
| Hanzi | `12` | IME activé avec le mode hanzi demi-largeur. |

### Exemples

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
            // Initialiser un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un contrôle ActiveX TextBox à la feuille de calcul
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Définir le mode IME sur Hiragana pleine largeur
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // Définissez d'autres propriétés à des fins de démonstration
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

            // Enregistrez le classeur
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


