---
title: "Shape.GetInputRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Ottiene l'intervallo utilizzato per riempire il controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/getinputrange/
---
## Shape.GetInputRange method

Ottiene l'intervallo utilizzato per riempire il controllo.

```csharp
public string GetInputRange(bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Valore di ritorno

L'intervallo utilizzato per riempire il controllo.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetInputRangeWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Input 1");
            worksheet.Cells["A2"].PutValue("Input 2");
            worksheet.Cells["A3"].PutValue("Input 3");

            // Aggiungi una forma di casella di riepilogo
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 0, 0);
            Shape shape = listBox;

            // Imposta l'intervallo di input per la casella di riepilogo
            shape.SetInputRange("$A$1:$A$3", false, false);

            // Ottieni l'intervallo di input
            string range = shape.GetInputRange(false, true);
            Console.WriteLine("Shape input range: " + range);
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


