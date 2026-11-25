---
title: "Enum EquationLimitLocationType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.Equations.EquationLimitLocationType enum. Specifica la posizione del limite su un operatore"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationlimitlocationtype/
---
## EquationLimitLocationType enumeration

Specifica la posizione del limite su un operatore.

```csharp
public enum EquationLimitLocationType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| UndOvr | `0` | Specifica che il limite è centrato sopra o sotto l'operatore. |
| SubSup | `1` | Specifica che il limite si trova sul lato destro dell'operatore. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationsClassEquationLimitLocationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi una forma di equazione al foglio di lavoro
                TextBox textBox = worksheet.Shapes.AddEquation(3, 0, 3, 0, 100, 200);

                // Ottieni il paragrafo dell'equazione e il suo primo figlio
                EquationNode mathNode = textBox.GetEquationParagraph().GetChild(0);

                // Crea un nodo di equazione Nary
                NaryEquationNode naryNode = (NaryEquationNode)mathNode.AddChild(EquationNodeType.Nary);

                // Imposta la posizione del limite su SubSup (lato destro dell'operatore)
                naryNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("Limit location set to SubSup: " + naryNode.LimitLocation);

                // Aggiungi del contenuto all'equazione
                EquationNode baseNode = naryNode.AddChild(EquationNodeType.Base);
                TextRunEquationNode textNode = (TextRunEquationNode)baseNode.AddChild(EquationNodeType.Text);
                textNode.Text = "x";

                // Cambia a UndOvr (centrato sopra/sotto l'operatore)
                naryNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("Limit location changed to UndOvr: " + naryNode.LimitLocation);

                // Salva la cartella di lavoro
                workbook.Save("EquationLimitLocationTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing.Equations](../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../)


