---
title: "NaryEquationNode.LimitLocation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NaryEquationNode. Questo attributo specifica la posizione dei limiti negli operatori nary. I limiti possono essere centrati sopra e sotto l'operatore nary o posizionati appena a destra dell'operatore"
type: docs
url: /it/net/aspose.cells.drawing.equations/naryequationnode/limitlocation/
---
## NaryEquationNode.LimitLocation property

Questo attributo specifica la posizione dei limiti negli operatori n-ari. I limiti possono essere centrati sopra e sotto l'operatore n-ario, oppure posizionati appena a destra dell'operatore.

```csharp
public EquationLimitLocationType LimitLocation { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class NaryEquationNodePropertyLimitLocationDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea una forma per contenere l'equazione
            var shape = worksheet.Shapes.AddEquation(0, 0, 200, 50, 200, 50);

            // Accedi all'equazione e aggiungi un nodo operatore nario
            var equation = shape.GetEquationParagraph();
            var naryNode = equation.AddChild(EquationNodeType.NaryEquation);

            // Esegui il cast a NaryEquationNode per accedere a LimitLocation
            var naryEquationNode = (NaryEquationNode)naryNode;

            try
            {
                // Mostra il LimitLocation corrente (valore predefinito)
                Console.WriteLine("Default LimitLocation: " + naryEquationNode.LimitLocation);

                // Imposta LimitLocation su SubSup (limiti sul lato destro)
                naryEquationNode.LimitLocation = EquationLimitLocationType.SubSup;
                Console.WriteLine("After setting to SubSup: " + naryEquationNode.LimitLocation);

                // Ritorna a UndOvr (limiti centrati)
                naryEquationNode.LimitLocation = EquationLimitLocationType.UndOvr;
                Console.WriteLine("After setting to UndOvr: " + naryEquationNode.LimitLocation);

                // Salva la cartella di lavoro
                workbook.Save("LimitLocationDemo.xlsx");
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

* enum [EquationLimitLocationType](../../equationlimitlocationtype/)
* class [NaryEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


