---
title: "ShapeCollection.CopyInRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ShapeCollection. Copia le forme nell'intervallo nell'intervallo di destinazione"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/copyinrange/
---
## ShapeCollection.CopyInRange method

Copia le forme nell'intervallo nell'intervallo di destinazione.

```csharp
public void CopyInRange(ShapeCollection sourceShapes, CellArea ca, int destRow, int destColumn, 
    bool isContained)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceShapes | ShapeCollection | Forme di origine. |
| ca | CellArea | L'intervallo di origine. |
| destRow | Int32 | L'indice della riga di destinazione dell'intervallo di destinazione. |
| destColumn | Int32 | La colonna di destinazione dell'intervallo di destinazione. |
| isContained | Booleano | Indica se copiare solo le forme contenute nell'intervallo. Se true, copia solo le forme nell'intervallo. Altrimenti, funziona come MS Office. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ottieni la collezione di forme
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi una forma rettangolare
            shapes.AddRectangle(2, 0, 2, 0, 130, 130);

            // Definisci l'area di celle da cui copiare
            CellArea area2 = new CellArea();
            area2.StartColumn = 1;
            area2.StartRow = 1;
            area2.EndColumn = 5;
            area2.EndRow = 11;

            // Copia le forme all'interno dell'intervallo specificato
            shapes.CopyInRange(shapes, area2, 12, 1, false);

            // Salva la cartella di lavoro
            workbook.Save("ShapeCopyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


