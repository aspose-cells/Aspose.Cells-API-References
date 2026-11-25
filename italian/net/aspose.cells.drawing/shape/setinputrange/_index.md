---
title: "Shape.SetInputRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Imposta l'intervallo usato per riempire il controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/setinputrange/
---
## Shape.SetInputRange method

Imposta l'intervallo utilizzato per riempire il controllo.

```csharp
public void SetInputRange(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | L'intervallo utilizzato per riempire il controllo. |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetInputRangeWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un oggetto cartella di lavoro
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle A1:A10
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Aggiungi una forma di casella di riepilogo
            Aspose.Cells.Drawing.Shape listBox = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);

            // Imposta l'intervallo di input per la casella di riepilogo (usando parametri String, Boolean, Boolean)
            listBox.SetInputRange("$A$1:$A$6", false, false);

            // Imposta la cella collegata per la casella di riepilogo
            listBox.SetLinkedCell("$A$12", false, true);

            // Salva la cartella di lavoro
            workbook.Save("SetInputRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


