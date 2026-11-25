---
title: "ShapeCollection.DeleteInRange"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapeCollection metodo. Elimina le forme nell'intervallo. Le forme di commento non saranno eliminate"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/deleteinrange/
---
## ShapeCollection.DeleteInRange method

Elimina le forme nell'intervallo.Le forme di commento non verranno eliminate.

```csharp
public void DeleteInRange(CellArea ca)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | CellArea | L'intervallo.Se le forme sono contenute nell'intervallo, saranno rimosse. |

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodDeleteInRangeWithCellAreaDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            // Aggiungi la prima forma rettangolare
            shapes.AddRectangle(2, 0, 2, 0, 50, 50);
            // Aggiungi la seconda forma rettangolare
            shapes.AddRectangle(6, 0, 2, 0, 30, 30);

            // Definisci l'intervallo in cui le forme devono essere eliminate
            CellArea area = new CellArea();
            area.StartColumn = 0;
            area.StartRow = 5;
            area.EndColumn = 5;
            area.EndRow = 8;

            // Elimina le forme all'interno dell'intervallo specificato
            shapes.DeleteInRange(area);

            // Salva la cartella di lavoro (opzionale)
            workbook.Save("ShapeDeleteInRangeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


