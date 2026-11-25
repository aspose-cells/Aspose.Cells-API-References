---
title: "Class GroupFill"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Drawing.GroupFill class. Rappresenta questo formato di riempimento che dovrebbe ereditare le proprietà di riempimento del gruppo"
type: docs
url: /it/net/aspose.cells.drawing/groupfill/
---
## GroupFill class

Rappresenta il formato di riempimento che dovrebbe ereditare le proprietà di riempimento del gruppo.

```csharp
public class GroupFill : Fill
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Ereditato da [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Ottiene il codice hash.(Ereditato da [`Fill`](../fill/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassGroupFillDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // GroupFill non espone un costruttore pubblico senza parametri.
                // Per scopi dimostrativi otteniamo un riferimento (null) del tipo.
                GroupFill groupFill = null;

                // Mostra che la variabile di tipo GroupFill esiste.
                Console.WriteLine($"GroupFill variable declared. Type: {typeof(GroupFill).FullName}");

                // Salva la cartella di lavoro (anche se non l'abbiamo modificata, questo dimostra un flusso di lavoro completo)
                workbook.Save("GroupFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with GroupFill: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


