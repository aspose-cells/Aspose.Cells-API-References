---
title: "ShapeCollection.AddGroupBox"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "ShapeCollection metodo. Aggiunge un GroupBox al foglio di lavoro"
type: docs
url: /it/net/aspose.cells.drawing/shapecollection/addgroupbox/
---
## ShapeCollection.AddGroupBox method

Aggiunge un GroupBox al foglio di lavoro.

```csharp
public GroupBox AddGroupBox(int topRow, int top, int leftColumn, int left, int height, int width)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| topRow | Int32 | Indice della riga in alto a sinistra. |
| alto | Int32 | Rappresenta lo spostamento verticale del GroupBox dalla sua riga sinistra, in unità di pixel. |
| leftColumn | Int32 | Indice della colonna in alto a sinistra. |
| sinistra | Int32 | Rappresenta lo spostamento orizzontale del GroupBox dalla sua colonna sinistra, in unità di pixel. |
| altezza | Int32 | Rappresenta l'altezza del GroupBox, in unità di pixel. |
| larghezza | Int32 | Rappresenta la larghezza del GroupBox, in unità di pixel. |

### Valore di ritorno

Un oggetto GroupBox.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddGroupBoxWithInt32Int32Int32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un group box al foglio di lavoro
            ShapeCollection shapes = worksheet.Shapes;
            Aspose.Cells.Drawing.GroupBox groupBox = shapes.AddGroupBox(1, 0, 1, 0, 100, 50);

            // Salva la cartella di lavoro
            workbook.Save("GroupBoxDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupBox](../../groupbox/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


