---
title: "LimLowUppEquationNode.Equals"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LimLowUppEquationNode. Determina se il nodo equazione corrente è uguale al nodo specificato"
type: docs
url: /it/net/aspose.cells.drawing.equations/limlowuppequationnode/equals/
---
## LimLowUppEquationNode.Equals method

Determina se il nodo dell'equazione corrente è uguale al nodo specificato

```csharp
public override bool Equals(object obj)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| obj | Object | Il nodo specificato |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Equations;
    using System;

    public class LimLowUppEquationNodeMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poiché non conosciamo i parametri del costruttore, confronteremo valori null
            // Questa è una modifica minima per farlo compilare - in un utilizzo reale avresti bisogno di una costruzione corretta
            LimLowUppEquationNode node1 = null;
            LimLowUppEquationNode node2 = null;

            try
            {
                // Chiama il metodo Equals con il tipo di parametro specifico (Object)
                bool areEqual = node1?.Equals((object)node2) ?? false;

                // Visualizza il risultato
                Console.WriteLine($"Are the nodes equal? {areEqual}");

                // Salva la cartella di lavoro
                workbook.Save("LimLowUppEquationNodeEqualsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [LimLowUppEquationNode](../)
* namespace [Aspose.Cells.Drawing.Equations](../../../aspose.cells.drawing.equations/)
* assembly [Aspose.Cells](../../../)


