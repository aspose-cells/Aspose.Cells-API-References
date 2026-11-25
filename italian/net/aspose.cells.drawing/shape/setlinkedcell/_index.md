---
title: "Shape.SetLinkedCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Shape. Imposta l'intervallo collegato al valore del controllo"
type: docs
url: /it/net/aspose.cells.drawing/shape/setlinkedcell/
---
## Shape.SetLinkedCell method

Imposta l'intervallo collegato al valore del controllo.

```csharp
public void SetLinkedCell(string formula, bool isR1C1, bool isLocal)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | String | L'intervallo collegato al valore del controllo. |
| isR1C1 | Booleano | Indica se la formula deve essere formattata come R1C1. |
| isLocal | Booleano | Indica se la formula deve essere formattata in base alla lingua locale. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeMethodSetLinkedCellWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi una forma di barra di scorrimento
            Aspose.Cells.Drawing.Shape scrollBar = worksheet.Shapes.AddScrollBar(2, 0, 2, 0, 130, 30);

            // Collega il valore della barra di scorrimento alla cella A12
            scrollBar.SetLinkedCell("$A$12", false, true);

            // Salva la cartella di lavoro
            workbook.Save("SetLinkedCellDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


