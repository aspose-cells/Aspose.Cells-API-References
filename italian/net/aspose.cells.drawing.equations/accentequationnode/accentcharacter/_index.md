---
title: "AccentEquationNode.AccentCharacter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AccentEquationNode. Questo attributo specifica il tipo di segno diacritico combinante collegato alla base della funzione di accento. Il carattere di accento predefinito è U0302. Si consiglia vivamente di utilizzare l'attributo AccentType per impostare il carattere di accento. Utilizza questa impostazione di proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto."
type: docs
url: /it/net/aspose.cells.drawing.equations/accentequationnode/accentcharacter/
---
## AccentEquationNode.AccentCharacter property

Questo attributo specifica il tipo di segno diacritico combinante collegato alla base della funzione di accento. Il carattere di accento predefinito è U+0302. Si consiglia vivamente di utilizzare l'attributo AccentType per impostare il carattere di accento. Utilizza questa impostazione della proprietà se non riesci a trovare il carattere di cui hai bisogno in un tipo noto.

```csharp
public string AccentCharacter { get; set; }
```

### Osservazioni

Va notato che questa proprietà accetta solo un carattere e, se vengono passati più caratteri, viene accettato solo il primo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Equations;

namespace AsposeCellsExamples
{
    public class AccentEquationNodePropertyAccentCharacterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi una forma di equazione al primo foglio di lavoro
            TextBox textBox = workbook.Worksheets[0].Shapes.AddEquation(3, 0, 3, 0, 100, 200);

            // Ottieni il nodo dell'equazione e aggiungi un nodo di accento
            EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);
            AccentEquationNode accentNode = (AccentEquationNode)mathNode.AddChild(EquationNodeType.Accent);
            
            // Imposta il carattere di accento (circonflesso in questo caso)
            accentNode.AccentCharacter = "\u0302";

            // Aggiungi il testo di base per l'accento
            EquationNode baseNode = accentNode.AddChild(EquationNodeType.Base);
            TextRunEquationNode textNode = (TextRunEquationNode)(baseNode.AddChild(EquationNodeType.Text));
            textNode.Text = "x";

            // Salva la cartella di lavoro
            workbook.Save("AccentEquationDemo.xlsx");

            // Verifica il file salvato ricaricandolo
            Workbook loadedWorkbook = new Workbook("AccentEquationDemo.xlsx");
            TextBox loadedTextBox = (TextBox)loadedWorkbook.Worksheets[0].Shapes[0];
            AccentEquationNode loadedAccentNode = (AccentEquationNode)loadedTextBox.GetEquationParagraph().GetChild(0).GetChild(0);
            
            // Emetti il carattere di accento per dimostrare la proprietà
            Console.WriteLine("Accent Character: " + loadedAccentNode.AccentCharacter);
        }
    }
}
```

### Vedi anche

* class [AccentEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


