---
title: "EquationNodeParagraph.Justification"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà EquationNodeParagraph. Specifica l'allineamento del paragrafo matematico, una serie di equazioni adiacenti all'interno dello stesso paragrafo. Un paragrafo matematico può essere Allineato a Sinistra, Allineato a Destra, Centrado o Centrado come Gruppo. Per impostazione predefinita il paragrafo matematico è Centrado come Gruppo. Ciò significa che le equazioni possono essere allineate tra loro, ma l'intero gruppo di equazioni è centrato nel suo complesso"
type: docs
url: /it/net/aspose.cells.drawing.equations/equationnodeparagraph/justification/
---
## EquationNodeParagraph.Justification property

Questo specifica l'allineamento del paragrafo matematico (una serie di equazioni adiacenti all'interno dello stesso paragrafo). Un paragrafo matematico può essere Left Justified, Right Justified, Centered, o Centered as Group. Per impostazione predefinita, il paragrafo matematico è Centered as Group. Ciò significa che le equazioni possono essere allineate tra loro, ma l'intero gruppo di equazioni è centrato nel suo complesso.

```csharp
public EquationHorizontalJustificationType Justification { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class EquationNodeParagraphPropertyJustificationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per contenere l'equazione
            var shape = worksheet.Shapes.AddTextBox(0, 0, 200, 50, 200, 50);

            // Ottieni il paragrafo dell'equazione
            var equationParagraph = shape.GetEquationParagraph() as EquationNodeParagraph;

            // Visualizza il valore di allineamento corrente
            Console.WriteLine("Current Justification value: " + equationParagraph.Justification);

            // Imposta valori di allineamento diversi e osserva gli effetti
            equationParagraph.Justification = EquationHorizontalJustificationType.Left;
            Console.WriteLine("Set to Left justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Center;
            Console.WriteLine("Set to Center justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.CenterGroup;
            Console.WriteLine("Set to CenterGroup justification");

            equationParagraph.Justification = EquationHorizontalJustificationType.Right;
            Console.WriteLine("Set to Right justification");

            // Salva la cartella di lavoro
            workbook.Save("EquationJustificationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [EquationHorizontalJustificationType](../../equationhorizontaljustificationtype/)
* class [EquationNodeParagraph](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


